# Azure-Sentinel---Live-Threat-Analysis
Azure Sentinel - Live Threat Analysis 
Implemented Azure Sentinel SIEM for cloud security. Used a live virtual machine as a honey pot to observe and analyze real-time RDP brute force attacks from around the world. Developed a custom PowerShell script to map attackers' geolocation information in Azure Sentinel.

The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.

The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map!

Languages Used
PowerShell: Extract RDP failed logon logs from Windows Event Viewer
Utilities Used
ipgeolocation.io: IP Address to Geolocation API
Attacks from China coming in; Custom logs being output with geodata


<img width="576" alt="Screenshot 2024-01-31 at 4 08 02 PM" src="https://github.com/johnjlopes20/Azure-Sentinel---Live-Threat-Analysis/assets/75873237/af61a9ff-ac8a-4c61-a448-02f52e319c00">


<img width="727" alt="Screenshot 2024-01-31 at 4 06 47 PM" src="https://github.com/johnjlopes20/Azure-Sentinel---Live-Threat-Analysis/assets/75873237/d7a7adc0-bb5b-42f9-8e95-7c5cc73c4ca5">



World map of incoming attacks after 24 hours (built custom logs including geodata)

![68747470733a2f2f692e696d6775722e636f6d2f6b725246724b352e706e67](https://github.com/johnjlopes20/Azure-Sentinel---Live-Threat-Analysis/assets/75873237/84f42902-5e03-40af-b0c7-323ba27f8d34)
