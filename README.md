<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

1. Enable Internet Information Services (IIS)
2. Install Web Platform Installer
3. Install MySQL and set up user and pass
4. Install C++ Redistributable
5. Configure permissions and install osTicket

<h2>Installation Steps</h2>
First you are going to create a Virtual machine, be sure to create a resource, name the resource group as well as the virtual machine name. Be sure to place your VM and resource group in the same region,(If place in different regions they will not be about to access one another). place images in windows 10, and the size to be atleast 2 VCPUS.
<P>
  
insert a Username and password within administrator account(this is for you solely to remember). click the Check box and Cream the VM
<p>
<img width="564" alt="image" src="https://github.com/user-attachments/assets/56902861-f981-47f9-8c32-a96397e06c62" />
<p>
<p>
<br />
<img width="619" alt="image" src="https://github.com/user-attachments/assets/d73378b9-831b-441c-8590-3fbb94b3e6fc" />
</p>
<p>
</p>
<img width="572" alt="image" src="https://github.com/user-attachments/assets/dabf8339-7739-4c85-94e9-7b43b41d8384" />
<p>
<p>    
</p>
<img width="647" alt="image" src="https://github.com/user-attachments/assets/88bda4f9-3d8e-4ab7-bb39-799d4b944fe6" />
<p>
<p>  
</p>
<img width="359" alt="image" src="https://github.com/user-attachments/assets/f890d9e5-5621-4e76-bff3-f54f6054f1b5" />


</p>
<p>
Once you create your virtual machine, it may take a moment to deploy. once the deployment is done, you can not start buy going to your desktop and open the virtual machine within your virtual desktop. 
</p>
<p>
<p>    
</p>
<img width="326" alt="image" src="https://github.com/user-attachments/assets/f74e21e7-c8af-447a-b995-40f46f9f1d92" />
<p>  
</p>
<p>
to gain access to the virtual desktop you now have to retreive the public IP address of the virtual machine and insert it into the remote desktop  
</p>
<p>  
</p>
<img width="100" alt="image" src="https://github.com/user-attachments/assets/bcebd823-de58-4a22-83f4-5975bbf982cb" />
<p>  
</p>
<img width="307" alt="image" src="https://github.com/user-attachments/assets/00228f6f-4256-4d5e-96ab-cb215bc2c11c" />
<p>  
</p>
</p>
this is where you enter the credentials, the username and password that you create within azures is what you want to insert here to gain access to the remote desktop
<p>
<p>
<img width="334" alt="image" src="https://github.com/user-attachments/assets/391bc2dc-7006-41fe-99d7-6b116a82a5b2" />
</p>
<p>
Within the Virtual machine, download the osTicket-Installation-Files.zip and unzip it onto your desktop, this will allow you to have the ability to install ostickets  
</p>
<p>
![image](https://github.com/user-attachments/assets/bcf405ce-f96b-484a-85bc-073d15a686e6)
  
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
