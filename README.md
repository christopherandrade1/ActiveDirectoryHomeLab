<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
In this project, I demonstrate the step-by-step process of establishing a fundamental Active Directory Home Lab and utilizing PowerShell to efficiently incorporate users.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>names.txt</b>

<h2>Environment Used </h2>

- <b>Oracle VirtualBox</b>
- <b>Windows Server</b>
- <b>Windows 10</b>

<h2>Project Overview:</h2>

Download VirtualBox, Windows Sever, Windows 10: <br/>

- <a href="https://www.virtualbox.org/wiki/Downloads">Oracle VirtualBox</a>
- <a href="https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019">Windows Server</a>
- <a href="https://www.microsoft.com/en-us/software-download/windows10">Windows 10</a>

<p align="center">
<br />
<br />
 
Start a packet capture on an ethernet port and save it to file: <br/>

- The wired interface includes the ethernet packet capture, which begins with ‘en’ in Wireshark
- The Wireshark app includes controls to start packet capture, stop capture, save the packets to a file, and load the capture file
- A capture can only be saved once the capture has stopped

<p align="center">
<br />

Use a display filter to detect HTTPS packets:  <br/>

- To display certain packets in an existing packet capture, use a display filter
- To display only HTTPS traffic, use a filter on TCP port 443: **tcp.port == 443**
 
<p align="center">
<br />

Visit a web page and detect its IP address using a display filter:  <br/>

- A TLS handshake display filter may be used to detect a website visit in a packet list: **tls.handshake.type ==1**
- The IP address is used in a filter to obtain packet information for a particular website: **ip.addr == 142.250.189.4**

<p align="center">
<br />
 
Locate all HTTPS packets from a capture not containing a certain IP address:  <br/>

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
