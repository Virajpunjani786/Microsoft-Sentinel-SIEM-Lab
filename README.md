# Microsoft-Sentinel-SIEM-Lab
Explore Microsoft Sentinel with this guide on my SIEM setup. I connected it to a live VM honeypot, detecting real-time attacks like RDP Brute Force worldwide. A custom PowerShell script identified attackers' geolocations, which I visualized on the Azure Sentinel map with detailed screenshots.

<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Microsoft Sentinel</b>

<h2>Project walk-through:</h2>


Setting up a VM in Azure: <br/>
<img src="https://i.imgur.com/sQo0YgM.png[/img]" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created firewall rules to accept all traffic:  <br/>
<img src="https://i.imgur.com/qSiAhXA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a Log Analytics workspace

<br />
<br />
 Connected Log Analytics to the VM
 <br />
 <br />
Setting up Sentinel, connecting the VM to it:  <br/>
<img src="https://i.imgur.com/hdGiEbI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connected to the VM through Remote Desktop:  <br/>
<img src="https://i.imgur.com/ZMp9VmB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Pinging the vm to make sure traffic can come through:  <br/>
<img src="https://i.imgur.com/GkZRWJX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Running a Powershell script (It pulls all the EventLog-SecurityLog, grabs all the events of all the failed logins and creates a new logfile):  <br/>
<img src="https://i.imgur.com/7xotPhX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Log that was created after running the script:  <br/>
<img src="https://i.imgur.com/bWbro4o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating a logfile to train log analytics what to look for in the logfile:  <br/>
<img src="https://i.imgur.com/O10T49w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Making sure the logs came through successfully:  <br/>
<img src="https://i.imgur.com/1scymYy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setting Up World MAP:  <br/>
<img src="https://i.imgur.com/rldHc8K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Checking Powershell script, noticed that people have discovered the VM and are trying to brute force
<img src="https://i.imgur.com/nyNNVZr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/RoodEet.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 
 
