<h1>Active Directory Lab</h1>

<h2>Description</h2>
This Lab consists of creating a virtual machine to act as a domain controller, which will contain the active directory. This VM will be given two network adapters, one will be used to connect to the internet and the other will connect to the virtual box private network that the "clients" will connect to. After the VM is created I will install Windows server 2019 on it and assign IP addresses to the internal network (the external network automatically gets an IP address from the home network). After IP addressing is set up, I name the server, then install Active Directory and create the domain. After, I configure NAT and routing to allow the clients on the private network to reach the internet through the DC. Then I will set up a DHCP on the DC, so when a Windows 10 machine is created i.e.(Client_1) the machine will be able to get an IP address. Then I run a powershell script to automatically create 1000 users for the Active Directory in the DC. Finally, I will create another VM and install Windows 10 on it which will be connected to the private virtual box network, the VM will be named "Client_1" and it will be joined to the domain, then I log into it with one of the domain accounts.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Powershell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility and create domain controller: <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20105637.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Section:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Section: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Section:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Section:  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
section:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Section:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
