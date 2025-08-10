<p align="center">
<img width="500" height="281" alt="image" src="https://github.com/user-attachments/assets/a8c3a3b5-73e9-4b90-b2de-b343a285bdd1" />
</p>
<h1>Domain Controller and Client VM Setup in Azure</h1>
This project involved setting up a domain controller (DC-1) on Windows Server 2025 and a client machine (Client-1) on Windows 11 within the same Azure virtual network. Key configurations included assigning a static private IP to the domain controller, modifying DNS settings on Client-1 to point to DC-1, and verifying successful network communication and DNS resolution using PowerShell tools.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure Portal
- Azure Virtual Network and Subnet
- PowerShell
- Remote Desktop Protocol (RDP)


<h2>Operating Systems Used </h2>

- Windows Server 2025 (DC-1)
- Windows 11 Pro VM (Client-1)

<h2>Key Tasks Performed:</h2>
<p>
• Created a Resource Group, Active-Directory-Lab, and deployed a Virtual Network with a Subnet, Active-Directory-VNet, to set up a structured, manageable, and secure network foundation in your cloud environment.

<br />
<p>
<img width="822" height="854" alt="image" src="https://github.com/user-attachments/assets/394f47ca-6fb9-4ebe-bd4b-196cc0786a0e" />
</p>
<p>
• Provisioned “DC-1” VM (Windows Server 2022) and set its NIC Private IP to static to maintain network stability and ensure the domain controller is always reachable at the same IP.

<br />
<p>
<img width="1051" height="272" alt="image" src="https://github.com/user-attachments/assets/23c63ccc-3265-49df-a7b7-81a1d3a7feca" /><br />
<img width="975" height="235" alt="image" src="https://github.com/user-attachments/assets/ef5593c3-1da8-441b-a58c-ead1388ba8b7" />
</p>
<p>
• Temporarily Disabled Windows Firewall on DC-1 to remove potential firewall barriers while testing network and domain functionality.

<br />
<p>
<img width="861" height="638" alt="image" src="https://github.com/user-attachments/assets/45eea650-f64e-4366-9755-d72328546c34" />
</p>

<p>
• Created “Client-1” VM (Windows 11), attached it to the same region and VNet as DC-1 set up a client machine that can securely and efficiently interact with your domain controller and other network resources.

<br />
<p>
<img width="975" height="492" alt="image" src="https://github.com/user-attachments/assets/3e0cc46b-923d-4956-83b0-f8e8af1b121f" />
</p>
<p>
• Verified connectivity by successfully pinging DC-1 from Client-1 using the ping command, making sure Client-1 and DC-1 are properly connected and ready for further domain-related tasks.

<br />
<p>
<img width="1084" height="605" alt="image" src="https://github.com/user-attachments/assets/472820f1-fdff-4eaa-a1f4-5bd2fea84f99" />
</p>
<p>
• Confirmed DNS settings on Client-1 using ipconfig /all in PowerShell to confirm that DNS settings are correctly configured for domain connectivity and troubleshooting.

<br />
<p>
<img width="1108" height="623" alt="image" src="https://github.com/user-attachments/assets/19d8d20b-7417-4363-a232-351fe48ea085" />
</p>

<p>
<b>Skills Demonstrated</b> <br />

  - Azure VM provisioning and network configuration
  - Static IP and DNS setup in virtual environments
  - Client-server connectivity troubleshooting
  - PowerShell command-line network diagnostics
  - Understanding of domain controller and DNS interactions

</p>
<br />
<p>
<b>Challenges & Solutions</b> <br />
<b>Challenge:</b> Ensuring proper DNS resolution between VMs <br />
<b>Solution:</b>  Assigned static IP to DC-1 and correctly configured Client-1’s DNS settings followed by restart to apply changes
</p>
<br />
<p>
<b>Results & Takeaways</b> <br />

  - Successfully configured a domain controller and client environment in Azure
  - Gained practical experience with virtual networking, DNS resolution, and connectivity validation
  - Strengthened skills in cloud-based infrastructure setup and testing
 </p>

