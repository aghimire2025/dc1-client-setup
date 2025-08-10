<p align="center">
<img width="624" height="426" alt="image" src="https://github.com/user-attachments/assets/cfeb03ff-fab0-4e1d-acee-92788c185730" />
</p>
<h1>Active Directory Domain Services Setup and User Management in Azure</h1>
This project involved promoting a Windows Server VM as a domain controller for a new forest (mydomain.com), configuring a client machine to join the domain, organizing directory objects into OUs, creating administrative and standard user accounts, and validating login access across systems. The project also included enabling Remote Desktop access for non-administrative users and automating bulk user creation using PowerShell.<br />
<h2>Environments and Technologies Used</h2>

- Microsoft Azure Portal
- Remote Desktop
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)
- PowerShell ISE

<h2>Operating Systems Used </h2>

- Windows 11 Pro (Client-1) </b> (21H2)
- Windows Server 2025 (DC-1)

<h2>List of Prerequisites</h2>

- Had an Azure subscription with VM creation rights
- Configured VNet with subnet for DC-1 and Client-1
- Deployed Windows Server 2025 (DC-1) & Windows 11 Pro (Client-1)
- Assigned static IP to DC-1 and allowed RDP (3389) in NSG
- Installed AD DS role & ADUC console
- Used PowerShell for scripting
- Prepared admin credentials and domain setup plan

<h2>Key Tasks Performed:</h2>
<p>

• Installed Active Directory Domain Services (AD DS) on Windows Server 2025 (DC-1) and promoted it to a domain controller for mydomain.com to make DC-1 the central authority for managing users, computers, and security settings in my network, then created two Organizational Units (OUs): _Employees, and _Admins in Active Directory Users and Computers (ADUC) to organize and manage directory objects more efficiently within Active Directory.

<br />
<p>
<img width="952" height="675" alt="image" src="https://github.com/user-attachments/assets/194be9d9-0148-48db-b91c-a630322f32d6" />
</p>
<p>

• Created a domain admin account, jane_admin for Jane Doe, and added her to the “Domain Admins” group to provide her with administrative privileges so that she can perform high-level administrative tasks. 

<br />
<p>
<img width="794" height="558" alt="image" src="https://github.com/user-attachments/assets/75200f90-6ab0-45c1-9659-847da1fa7c2e" />
</p>
<p>
<img width="952" height="675" alt="image" src="https://github.com/user-attachments/assets/194be9d9-0148-48db-b91c-a630322f32d6" />
</p>
<p>

• Created a domain admin account, jane_admin for Jane Doe, and added her to the “Domain Admins” group to provide her with administrative privileges so that she can perform high-level administrative tasks. 

<br />
<p>
<img width="794" height="558" alt="image" src="https://github.com/user-attachments/assets/75200f90-6ab0-45c1-9659-847da1fa7c2e" />
</p>
<p>

• Logged into Windows Server 2025 (DC-1) as Jane_admin then Joined Windows 11 Pro (Client-1) to the domain by logging in to Client-1 VM. Client-1 has shown up in Active Directory Users and Computers (ADUC) in DC-1 to connect the Windows 11 Pro machine (Client-1) to my  Active Directory domain, so it could be centrally managed through the Domain Controller (DC-1)

<br />
<p>
<img width="920" height="645" alt="image" src="https://github.com/user-attachments/assets/06c84615-4095-4a0a-b099-035f2b734482" />
</p>
<p>

• Created a domain admin account, jane_admin for Jane Doe, and added her to the “Domain Admins” group to provide her with administrative privileges so that she can perform high-level administrative tasks. 

<br />
<p>
<img width="794" height="558" alt="image" src="https://github.com/user-attachments/assets/75200f90-6ab0-45c1-9659-847da1fa7c2e" />
</p>
<p>

• Enabled Remote Desktop access on Client-1 for “Domain Users” group so that any user account in the “Domain Users” group (basically, all regular Active Directory users) can remotely log in to Client-1 via Remote Desktop Protocol (RDP), allowing domain-wide remote access.

<br />
<p>
<img width="883" height="584" alt="image" src="https://github.com/user-attachments/assets/bbe6182f-47c4-4723-95cb-c0cd97bb2841" />
</p>
<p>

• Used a PowerShell script to create multiple standard user accounts under _EMPLOYEES OU to efficiently set up multiple employee accounts in a structured, organized, and consistent way within Active Directory, and observed multiple accounts being created.
<br />
<p>
<img width="882" height="603" alt="image" src="https://github.com/user-attachments/assets/a73707f5-a034-4484-99c5-4debbfe6a224" />
<img width="650" height="597" alt="image" src="https://github.com/user-attachments/assets/444f61e4-7861-4b40-99b5-c7550e1a0ee4" />
</p>
<p>

• Successfully logged into Client-1 using a standard domain user account “batu.sege”

<br />
<p>
<img width="683" height="631" alt="image" src="https://github.com/user-attachments/assets/67a3db47-0911-4308-9f91-21be083b3e65" />
</p>
<p>
<b>Skills Demonstrated</b> <br />

  - Active Directory installation and domain configuration
  - Domain user and group management in ADUC
  - Client PC domain joining and remote access configuration
  - PowerShell scripting for user account automation
  - Organizational Unit structure and permission delegation
  - Azure VM lifecycle management and cost-saving practices

</p>
<br />
<p>
<b>Challenges & Solutions</b> <br />
<b>Challenge:</b>  Allowing Remote Desktop for non-admin domain users <br />
<b>Solution:</b>  Configured RDP settings on Client-1 to grant access to the “Domain Users” group
</p>
<br />
<p>
<b>Results & Takeaways</b> <br />

  - Successfully deployed and configured AD DS in an Azure-hosted environment
  - Gained practical experience with user account management, group policies, and domain-joined infrastructure
  - Strengthened understanding of enterprise-level directory services and access control principles
 </p>

