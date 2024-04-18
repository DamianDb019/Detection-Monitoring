<h1>Detection & Monitoring Setup Lab</h1>


<h2>Description</h2>
This is a lab I recreated for offensive and defensive security.

My purpose for this lab is to learn more about Security Monitoring and Detection Engineering.
<br />


<h2>Languages and ISO's Used</h2>

- <b>Bash</b>
- <b><a href="https://www.pfsense.org/download/">pfsense<a/></b>
- <b><a href="https://github.com/Security-Onion-Solutions/securityonion/blob/master/VERIFY_ISO.md">Security Onion</a></b>
- <b><a href="https://ubuntu.com/download/desktop">Ubuntu Desktop</a></b>
- <b><a href="https://www.offensive-security.com/kali-linux-vm-vmware-virtualbox-image-download/">Kali Linux</a><b/>
- <b><a href="https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019">Windows 2019 Server Eval Copy</a></b>
- <b><a href="https://www.microsoft.com/en-us/evalcenter/evaluate-windows-10-enterprise">Windows 10 Eval Copy</a></b>
- <b><a href="https://ubuntu.com/download/server">Ubuntu Server</a></b>

<h2>Virtual Machines Used </h2>

<b>~ Kali: This is the offensive machine that will be used to propagate different forms of attacks.

~ pfsense: This will be the firewall for controlling inbound and outbound traffic, only accessible and visible in the VM private network.

~ Security Onion: This will be the all-in-one IDS, Security Monitoring, and Log Management solution.

~ Splunk: This is an additional SIEM that will be used in addition and comparison to Kibana on Security Onion.

~ Windows 2019 Server: This will be the Windows domain controller that will have two Windows machines connected to it.

~ Windows 10: These Windows machines will vary based on individual needs.

~ Ubuntu machines: Linux machines that can be added to the network for exploitation, detection, or monitoring purposes.</b>

<h2>Recap of my Progress through the Lab:</h2>

<p align="center">
pfsense setup: <br/>
<img src="https://i.imgur.com/4WACs00.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
SecOnion Alerts:  <br/>
<img src="https://i.imgur.com/hI0xHnA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Firewall created in the pfsense WebConfigurator: <br/>
<img src="https://i.imgur.com/J3zjHEn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set up a bridge between VictimNetwork and ScanPort:  <br/>
<img src="https://i.imgur.com/Y5WIxbs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set up Windows Server 2019 w/ AD Domain Services, AD Certificate Roles| Configured the IPv4 to be my VictimsNetwork:  <br/>
<img src="https://i.imgur.com/jglCMqU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Complete set up Windows Server 2019:  <br/>
<img src="https://i.imgur.com/mpilkWR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Completed a Powershell script to create 1000 AD users with passwords:  <br/>
<img src="https://i.imgur.com/Hoe9ggx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Showing accounts created along with the OU:  <br/>
<img src="https://i.imgur.com/UFEZdDX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created two Windows 10 machines and connected to the Domain:  <br/>
<img src="https://i.imgur.com/irGBbYZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Installed Splunk from splunk.com and untar with bash | Installed net-tools as well:  <br/>
<img src="https://i.imgur.com/SMK4BS9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
DC nor the Windows Desktops had Internet created a rule in the firewall pfsense to allow:  <br/>
<img src="https://i.imgur.com/UrVYEIF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe Splunk for forwarded Eventlogs from DC and Workstations:  <br/>
<img src="https://i.imgur.com/dMKrLPl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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

