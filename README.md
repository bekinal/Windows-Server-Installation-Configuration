<h1>Windows Server 2016 Configuration</h1>

<h2>Description</h2>
Project consists of adding the Active Directory Domain Services feature to Windows Server 2016. A seperate server (Standard Evaluation) is then added to the domain. 
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2016</b>

<h2>Environments Used </h2>

- <b>Windows Server 2016</b>

<h2>Windows Server 2016 (GUI):</h2>

 Open the Server Manager Dashboard and select "Manage", "Add Roles and Features". 
 Click next until you reach the "Select server roles" tab: <br/>
<img src="https://i.imgur.com/g0YrjO1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select "Active Directory Domain Service" and click "Add Features":  <br/>
<img src="https://i.imgur.com/w35sWrV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Continue through - Click "Install": <br/>
<img src="https://i.imgur.com/g3ShiHN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Return to dashboard and click the flag. Select "Promote this server to a domain controller":  <br/>
<img src="https://i.imgur.com/1O8KPgf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter "cyber.local" in root domain name and click next. Include a password for the CYBER\administrator account:  <br/>
<img src="https://i.imgur.com/qVdQuyB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Proceed next and then install:  <br/>
<img src="https://i.imgur.com/DkJ4Yvs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
System will restart. Log in with the CYBER\administrator credentials:  <br/>
<img src="https://i.imgur.com/WNcPbr7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>Windows Server 2016 (Standard Evalutation):</h2>
Type "sconfig" to enter the configuration options: <br/>
<img src="https://i.imgur.com/y4j5940.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Select option 1 to enter into a Domain with the letter D. Enter the Domain name "cyber.local", then the authorized domain user, cyber\administrator:  <br/>
<img src="https://i.imgur.com/vAZ0ewM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Type in the password for the administrator. When typing the password, notice that nothing will populate the screen. Hit enter, and select No when prompted to name change. Restart the machine:  <br/>
<img src="https://i.imgur.com/80KLDOr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
