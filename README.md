<p align="center">
<img src="https://i.imgur.com/G0Ls18P.png"/>
</p>

<h1>Group Policy Management</h1>
In this tutorial, we configure an account lockout policy in Active Directory using Group Policy Management.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Group Policy Management Console
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Add Group Policy Objects
- Configure Account Lockout Policy
- Verify Policy

<h2>Configuration Steps</h2>

![image](https://github.com/user-attachments/assets/9e9d5ee7-21dd-4f5e-89a5-cfb724547c9e)

<p>
In the Group Policy Management locate "Group Policy Objects" and add a new policy called "Account Lockout Policy"
</p>
<br />

![image](https://github.com/user-attachments/assets/65857da6-1625-42f7-bd9f-fa606bc5c2ca)

<p>
Edit the newly created policy and navigate to "Account Lockout Policy" and configure policy as needed.
</p>
<br />

![image](https://github.com/user-attachments/assets/a3e33e0b-f740-4e79-ba45-3a2a62bfcce3)

<p>
Link the organizational unit/domain to the new policy that was created
</p>
<br />

![image](https://github.com/user-attachments/assets/a6d13c02-71fe-4ef8-bbb5-32d18fd06c93)

<p>
Manually update the Group Policy by opening Powershell and inputting the command "gpudate /force". Then run command "rsop.msc" to verify that the policy has been applied.
</p>
