# 4. Adding Windows Event Logs
The Windows UF does not support the `add windows-event-log` command.  
Instead, I manually created the following file:

`C:\Program Files\SplunkUniversalForwarder\etc\system\local\inputs.conf`

With this content:

[WinEventLog://System]
disabled = 0

[WinEventLog://Application]
disabled = 0

[WinEventLog://Security]
disabled = 0


Then I restarted the UF again.

## 5. Verifying Data Flow

To verify that logs were being forwarded, I ran:

"C:\Program Files\SplunkUniversalForwarder\bin\splunk.exe" list monitor


And on my Splunk server, I searched:

index=* host=<windows-hostname>


I confirmed that Windows Event Logs were successfully ingested.



