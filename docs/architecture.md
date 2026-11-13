# SOC Lab – Architecture

## 1. Windows 11 Host
- Acts as the monitored endpoint.
- Generates Windows Security Events.
- Runs Sysmon for process monitoring.
- Runs Splunk Universal Forwarder to send logs.

## 2. VirtualBox
- Provides the virtual environment.
- Hosts the Ubuntu virtual machine.

## 3. Ubuntu 24.04 VM
- Runs Splunk Enterprise.
- Receives and indexes logs from Windows.

## 4. Data Flow

Windows Security Logs + Sysmon  
↓  
Splunk Universal Forwarder  
↓  
Splunk Enterprise on Ubuntu  
↓  
Log Search, Detection, Investigation and Reporting

## 5. Project Goal
Build a controlled SOC environment to monitor Windows activity, detect suspicious behaviour, investigate security events and document findings.