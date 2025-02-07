<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- The Setup of Active Directory 
- Server Manager
- Active Directory Users and Computers
- Group Policy and Managing Accounts

<h2>Deployment and Configuration Steps</h2>

![image](https://github.com/user-attachments/assets/832650f8-dcbc-43c3-9a1e-f77439eb6b4a)


<p>
</p>
<p>
I created one virtual machine that is running Windows Server, and it acts as our domain server. I created a second virtual machine that is running Windows 10, and it acts as a client that will join the domain. This helps simulate a client. 
</p>
<br />

![image](https://github.com/user-attachments/assets/c0d73824-b0a7-4afd-97f1-a11f5876ee62)

<p>
</p>
<p>
I’m inside the domain controller under the Server Manager. I installed Active Directory domain services. I added roles and features. I set up the server roles and configured the computer to be the new domain controller and adding a new forest. 
</p>
<br />

![image](https://github.com/user-attachments/assets/1061feb9-00b4-496b-9c94-59f0ab105990)

<p>
</p>
<p>
Under Active Directory Users and Computers, I created an organizational unit. One called Employees and another called Admin.  I also created a new user to fall under one of the organizations. 
</p>
<br />

![image](https://github.com/user-attachments/assets/deab97f8-46e3-4f24-bffd-39af9a118a6c)

<p>
</p>
<p>
I set up group policies and, more specifically, how many failed login attempts an individual would have before the account would be locked out. I went to the individual that was locked out because of the failed login attempts and unlocked the account.  
