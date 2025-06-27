<p align="center">
<img src="https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/ProtonVPNLogo.jpeg" height="40%" width="70%"alt="ProtonVPN Logo"/>
</p>

<h1>VPN Setup in a Virtual Machine</h1>
This walkthrough involves setting up a Virtual Machine in Azure. We will then access the VM using Remote Desktop, compare public IP addresses between the host and VM, and demonstrate how to install and configure Proton VPN on the VM. Finally, we'll verify the VPN connection by observing the change in the VM’s public IP address.<br />


<h2>Environments Used</h2>

- Microsoft Azure
- macOS (Host Machine)
- Windows 10 (Virtual Machine)
- Windows App (Remote Desktop)

<h2>Technology/Applications/Services </h2>


- Azure Virtual Machines
- whatismyipaddress.com




<h2>Walkthrough</h2>



Create a Windows 10 Virtual Machine on Azure

  
![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic1.png)
</p>
<br />
<p>
Log-in to the Virtual Machine using Windows App(Remote Desktop)
  


![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic2.png)
</p>
<br />
<p>
On the host system, go to https://whatismyipaddress.com. Note the Public IP Address.<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- For learning purposes, let's refer to Public IP Address of host as “A”

</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic3.png)
</p>
<br />
<p>
If we do the same on the Windows 10 VM, we see a different Public IP Address, “B”.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic4.png)
</p>
<br />
<p>
Now we will sign up for Proton VPN on our host machine.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic5.png)
</p>
<br />
<p>
We will be given a new password, or we can choose our own.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic6.png)
</p>
<br />
<p>
Instead of downloading the client in the host machine, we will do it in the Windows VM.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic7.png)
  
</p>
<br />
<p>
On the Windows VM we log in(not really necessary since we will do it again on VPN software).
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic8.png)
</p>
<br />
<p>
Download the Windows VPN client, the software that establishes connection/tunnel between the VM and the VPN servers.

</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic9.png)
</p>
<br />
<p>
Click install.
  
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic10.png)
</p>
<br />
<p>
We log in again in the VPN software.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic11.png)
</p>
<br />
<p>
We can click quick connect and connect to a random server.
</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic12.png)
</p>
<br />
<p>
If we check again on https://whatismyipaddress.com, we will see a different Public IP Address “C”, from the Host “A” and the VM “B.”

</p>



![image alt](https://github.com/GursimarJ/VPN-setup-and-usage/blob/a6f1ff3a97d1527ade2a67c96bacfea5a611f497/assets/Part6Pic13.png)
