<h1>Failed RDP attempts Live Map</h1>


<h2>Description</h2>
<b>
The PowerShell script available in this repository is in charge of extracting details from the Windows Event Log related to unsuccessful RDP attempts. Additionally, it utilizes a third-party API to gather geographical information concerning the location of the attackers.
</b>
<br />
<br />

In this demo, I'm utilizing a script to set up Azure Sentinel (SIEM) and link it to a live virtual machine functioning as a honey pot. We'll be witnessing real-time attacks, specifically RDP Brute Force attacks, coming in from various locations globally. I utilized a personalized PowerShell script to retrieve the geolocation details of the attackers and display them on an Azure Sentinel Map.
<br />
<br />


<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Live attacks detected from the Netherlands; log output on PowerShell</h2>

<p align="center">
<img src="https://i.imgur.com/9Co9oO3.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/T6xVoBI.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
