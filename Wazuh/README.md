# Wazuh Homelab

## Objective

- **Deploy and configure a Wazuh SIEM** on an **Ubuntu VM** to monitor host activity.
- **Register a Windows host as an agent** to enable centralized event collection and monitoring.
- **Implement File Integrity Monitoring (FIM)** to detect and alert on unauthorized file changes within the Windows system.
- **Understand** how the concepts of **endpoint telemetry, rule-based detection, and alert correlation** work in a real-world environment.

### Skills Learned

- **SIEM Deployment & Configuration**: Installed and configured the Wazuh server on Ubuntu and connected it with the web UI (via Wazuh Dashboard). 

- **Agent Registration**: Added and configured the Windows host as a Wazuh agent, establishing secure communication with the Wazuh manager. 

- **File Integrity Monitoring (FIM)**: Implemented FIM rules to monitor file changes, additions, and deletions on the Windows system. 

- **Log Analysis & Alert Management**: Analyzed alerts generated from monitored files and tuned rules for relevant detections. 

### Tools Used

- Ubuntu VM
- Windows Host
- Wazuh

## Findings

<img width="1277" height="797" alt="0 9" src="https://github.com/user-attachments/assets/cf26bc80-bb2f-4cb3-9aff-e7e417c0f7b5" />

In my Ubuntu VM, I ensured that the Windows Host is correctly configured as an agent in my Ubuntu VM Wazuh server.
***
<img width="317" height="277" alt="2" src="https://github.com/user-attachments/assets/eef8efb8-9de8-4f9d-8511-4ec6cdda6e45" />

On my Windows Host, I ensured my Windows Host is connected and running in my Ubuntu VM Wazuh server.
***
<img width="1276" height="796" alt="1" src="https://github.com/user-attachments/assets/4b382959-34d5-4fb8-b98a-4bcf0437e84a" />
<img width="1278" height="797" alt="1 1" src="https://github.com/user-attachments/assets/3b694b71-5aec-4283-a87f-4c747b82e64f" />
<img width="1279" height="797" alt="3" src="https://github.com/user-attachments/assets/624428a5-4e33-4d0e-a551-5f51067ca0ef" />
<img width="1278" height="798" alt="4" src="https://github.com/user-attachments/assets/de0e6321-885d-4445-a72f-ed3f00e5eef0" />

In my Ubuntu VM, I logged into my Wazuh server and checked File Integrity Management (FIM): Recent events for my Windows Host. There are currently no events.
***
<img width="911" height="711" alt="5" src="https://github.com/user-attachments/assets/2230404d-ff6a-41c0-93de-219ed13c2c79" />

On my Windows Host, I configured FIM for my desired directory.
***
<img width="1049" height="768" alt="6" src="https://github.com/user-attachments/assets/90fb2327-a1f3-4fa4-bd07-0073fac78a2e" />
<img width="1050" height="769" alt="6 1" src="https://github.com/user-attachments/assets/94c3a304-c4f6-4ecb-8f67-a328971b968d" />
<img width="1281" height="799" alt="6 2" src="https://github.com/user-attachments/assets/32f0555e-4ec3-4536-a8d3-039289abd39b" />

On my Windows Host, I deleted Test 1.

In my Ubuntu VM, I checked FIM: Recent events for my Windows Host. New events are shown above.
***
<img width="1050" height="769" alt="7" src="https://github.com/user-attachments/assets/ff6ee9d0-1fe3-40f0-bc0b-cdc658647036" />
<img width="1278" height="797" alt="7 1" src="https://github.com/user-attachments/assets/ed69d0f1-8254-40d8-b886-e8f2e9aad425" />

On my Windows Host, I created a New Test Document.

In my Ubuntu VM, I checked FIM: Recent events for my Windows Host. New events are shown above.

***
<img width="1047" height="767" alt="8" src="https://github.com/user-attachments/assets/6ee94440-de16-49dc-8d57-526d33f9c115" />
<img width="1278" height="798" alt="8 1" src="https://github.com/user-attachments/assets/6ec192dc-eff9-44c5-abb7-734d75c1f7b0" />

On my Windows Host, I Modified New Test Document.

In my Ubuntu VM, I checked FIM: Recent events for my Windows Host. New events are shown above.
