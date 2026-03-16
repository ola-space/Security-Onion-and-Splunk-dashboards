# Splunk SIEM Log Collection and Security Event Analysis

---


## Overview   
This project demonstrates the implementation of a Security Information and Event Management (SIEM) environment using Splunk Enterprise and Splunk Universal Forwarder. Logs from a Windows Server virtual machine were collected using the Splunk Universal Forwarder and forwarded to the Splunk Enterprise instance for indexing and analysis.   
  
The objective of this simulation is to demonstrate how security analysts collect, monitor, and analyze logs to detect suspicious activities in enterprise environments.   

A detailed setup guide and analysis report are included in this repository.

---

## Tools Used
* Splunk Enterprise
* Splunk Universal Forwarder
* Windows Server (Virtual Machine)

---

## Lab Summary

The SIEM lab environment was configured to collect Windows system logs from a virtual machine using Splunk Universal Forwarder and send them to Splunk Enterprise for analysis.   

Logs were monitored to validate that events generated on the Windows server were successfully forwarded and indexed in Splunk.   
Security events such as log clearing were simulated to confirm that the logging pipeline was functioning correctly.

--- 

## Methodology

The following steps were performed to implement the SIEM simulation:

- Installed Splunk Enterprise on the host machine.
- Installed Splunk Universal Forwarder on a Windows Server virtual machine.
- Placed the forwarder installer in a shared folder accessible to the VM for installation.
- Configured inputs.conf to collect Windows event logs.

Saved the configuration file in:
```
C:\Program Files\SplunkUniversalForwarder\etc\system\local\
```

- Configured the forwarder to send logs to the Splunk Enterprise server.
- Created firewall rules to allow outbound log forwarding traffic.
- Verified that logs from the Windows server were successfully received and indexed in Splunk Enterprise.

---

## Analysis Summary
This simulation demonstrates how logs generated on a Windows system are forwarded to Splunk and analyzed for security events.

During the analysis phase:

- Windows security logs were monitored in Splunk.
- The Windows security log was intentionally cleared to confirm that the event would be captured by the SIEM system.
- Splunk successfully detected the log-clearing activity, confirming that the logging pipeline and detection capability were functioning correctly.
- Additionally, detection alerts can be configured based on threat detection strategies such as those recommended by the **MITRE ATT&CK framework.

---


## **Project Report**

The complete report can be found here:

[Splunk Enterprise and Forwarder Setup Guide](https://github.com/ola-space/Security-Onion-and-Splunk-dashboards/blob/main/Splunk%20Enterprise%20and%20Forwarder%20Setup%20Guide.pdf)   
[Splunk Simulation Analysis Report](https://github.com/ola-space/Security-Onion-and-Splunk-dashboards/blob/main/Splunk%20Simulation%20Analysis%20Report.pdf)


---


## Author
**Olanipekun Babatunde**  
Cybersecurity Analyst
