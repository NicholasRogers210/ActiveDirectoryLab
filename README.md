<h1>Active Directory Lab</h1>

<h2>Description</h2>
In this lab, we will embark on the creation of a virtual machine that will serve as a domain controller, housing the Active Directory. To establish connectivity, the VM will be equipped with two network adapters. One adapter will facilitate internet access, while the other will connect to the virtual box private network, enabling the "clients" to connect. 

Once the VM is successfully created, we will proceed to install Windows Server 2019 and configure IP addresses for the internal network. The external network will automatically acquire an IP address from the home network. With the IP addressing in place, we will assign a name to the server and proceed to install Active Directory, thereby creating the domain. 

To ensure seamless internet access for the clients on the private network, we will configure NAT and routing. Additionally, a DHCP will be set up on the domain controller, allowing any Windows 10 machine, such as "Client_1," to obtain an IP address. 

To expedite the process of user creation within the Active Directory, we will execute a PowerShell script that will generate 1000 users. This will enhance the functionality of the domain controller. 

Lastly, we will create another virtual machine and install Windows 10 on it. This machine, named "Client_1," will be connected to the private virtual box network and joined to the domain. We will then log into "Client_1" using one of the domain accounts, completing the setup.

<br />


<h2>Languages and Utilities Used</h2>

- <b>Powershell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the virtual box and create the VM which will act as the domain controller: <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20105637.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Add two network adapters, one internal and one external:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20112609.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Assign IP addresses to the internal network: <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20113704.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Name the server and install the Active Directory:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20113924.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Configure NAT and routing to allow the clients on the private network to reach the internet through the DC:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20121554.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Set up a DHCP Server on the DC, so when a Windows 10 machine is created i.e.(Client_1) the machine will be able to get an IP address:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-11%20121957.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Run a PowerShell script to automatically create 1000 users for the Active Directory in the DC:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-12%20010651.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Create another VM and install Windows 10 on it, which will be connected to the private Virtual Box Network:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-12%20144146.png" height="80%" width="80%" alt="Active Directory Lab"/>
<br />
<br />
Client_1 connecting to the internet through the DC:  <br/>
<img src="https://github.com/NicholasRogers210/ActiveDirectoryLab/blob/main/Images/Screenshot%202023-07-12%20021732.png" height="80%" width="80%" alt="Active Directory Lab"/>
</p>
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
