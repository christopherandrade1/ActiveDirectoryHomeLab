<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
In this project, I demonstrate the step-by-step process of establishing a fundamental Active Directory Home Lab and utilizing PowerShell to efficiently incorporate users.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>names.txt</b>

<h2>Environment Used </h2>

- <b>Oracle VirtualBox</b>
- <b>Windows Server 2019</b>
- <b>Windows 10</b>

<h2>Project Overview:</h2>

Download VirtualBox, Windows Sever 2019, Windows 10: <br/>

- <a href="https://www.virtualbox.org/wiki/Downloads">Oracle VirtualBox</a>
- <a href="https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019">Windows Server 2019</a>
- <a href="https://www.microsoft.com/en-us/software-download/windows10">Windows 10</a>

<br />

Install Windows Server 2019: <br/>

- The wired interface includes the ethernet packet capture, which begins with ‘en’ in Wireshark

<p align="center">
<br />
<img src="https://imgur.com/XvVgU7n.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<img src="https://imgur.com/OZ2n8zH.png" height="80%" width="80%" alt="Installation Steps"/>
<br /> 

Insert Guest Additions in Windows Server:  <br/>

- To display certain packets in an existing packet capture, use a display filter
- To display only HTTPS traffic, use a filter on TCP port 443: **tcp.port == 443**
 
<p align="center">
<br />
<img src="https://imgur.com/9EdEnAc.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<img src="https://imgur.com/Rlc0ayu.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<img src="https://imgur.com/mWaEl7R.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<img src="https://imgur.com/IPQQMNl.png" height="80%" width="80%" alt="Installation Steps"/>
<br />

Rename the Networks:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Change System Name:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

Include Active Directory Service:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Create Administrative Account:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

Install NAT:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Install DHCP:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

Download Script:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Execute Script:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

Install Windows 10 in VirtualBox:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Check if IP is working:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

Change Windows 10 Name:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Sign-in with User Account:  <br/>

- A Conditional statement may be used to include and eliminate packets from a Wireshark capture: **!(ip.addr == 8.43.85.97) and tcp.port == 443**
- A compound conditional should include parentheses to avoid order of execution errors: **!(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)**

<p align="center">
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
- **Multimodal Encoding Stage.** Leveraging established encoders to encode inputs in various modalities, where these representations are projected into language-like representations comprehensible to the LLM through a projection layer.
<img src="https://imgur.com/geP0kkD.png" height="80%" width="80%" alt="Installation Steps"/>
```
--!>
