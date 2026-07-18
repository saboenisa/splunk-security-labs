# Splunk Security Lab

## Overview

This project documents the creation of a personal cybersecurity lab environment using Splunk.

The purpose of this lab is to gain hands-on experience with Security Information and Event Management (SIEM), log collection, security monitoring, and threat detection.

The environment simulates a small enterprise network where endpoints generate security events that are collected, indexed, searched, and analyzed using Splunk.

---

# Objectives

The main goals of this project are:

- Build a complete Splunk lab environment from scratch
- Understand Splunk architecture and components
- Configure data collection from Linux and Windows systems
- Learn how Universal Forwarders work
- Practice Search Processing Language (SPL)
- Create security alerts and detections
- Perform basic security investigations

---

# Lab Environment

The lab is built using:

| Component | Technology |
|---|---|
| Host Machine | Linux Laptop |
| Virtualization | Oracle VirtualBox |
| SIEM Platform | Splunk Enterprise |
| Linux Server | Ubuntu Server |
| Endpoint System | Windows 11 |

---

# Architecture

The environment consists of:
             Windows 11 Endpoint
                    |
                    |
          Splunk Universal Forwarder
                    |
                    |
             Splunk Server
                    |
                    |
      Search, Detection & Investigation


## Virtual Machines

| Hostname | Operating System | Role |
|---|---|---|
| Splunk | Linux Server | Splunk Enterprise Server |
| Splunk FWD | Linux Server | Forwarding logs to Splunk |
| SplunkWindows | Windows 11 | Endpoint generating events |

---

# Skills Practiced

## Splunk Administration

- Installing Splunk Enterprise
- Managing Splunk instances
- Understanding indexes and data inputs
- Performing upgrades

## Data Collection

- Installing Universal Forwarders
- Configuring log forwarding
- Collecting Windows Event Logs
- Collecting Linux system logs

## Security Monitoring

- Writing SPL searches
- Creating alerts
- Investigating events
- Building detections

---

# Project Structure

01-lab-setup
Lab architecture and virtual machine configuration

02-splunk-installation
Splunk installation guides

03-data-forwarding
Configuring data sources and forwarders

04-forwarders
Forwarder administration

05-splunk-administration
Splunk management notes

06-search-processing-language
SPL queries and examples

07-security-monitoring
Detection and investigation exercises
