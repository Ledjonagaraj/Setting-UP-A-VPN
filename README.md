# Vitual Private Network (VPN)
<p align="center">
<img src="https://i.imgur.com/Im4NjRa.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation using a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Windows App for Mac (previously named Microsoft Remote Desktop)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating IP Through VM (Italy)
- STEP 4 - Connecting to VPN Through VM
- STEP 5 - Locating IP Through VPN (Netherlands)

<h2>Installation Steps</h2>

STEP 1 - Locate your own personal IP address by going to "www.showmyip.com" which will be able to show you your local IP address. We will use this later as well. See EXAMPLE 1A below.

EXAMPLE 1A
<p>
<img src="https://i.imgur.com/cCTydeW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will set up a virtual machine on Azure. 
  
</p>
<br />

STEP 2 - Go to www.portal.azure.com and find Virtual Machines. (Create a free account with $200 if you need to). See Example 2A looking at the Virtual Machine set up page. 

EXAMPLE 2A
<p>
<img src="https://i.imgur.com/OV9Hh6t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Creating the Virtual Machine on Example 2B the VM as “VM-ItalyNorth” and select that for the REGION as well. Ensure the other items are selected as shown in EXAMPLE 2B & 2C.

EXAMPLE 2B
<p>
<img src="https://i.imgur.com/vElOmzc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

For the Username and Password you can create your custom information, just record it personally.
  
</p>
<br />

EXAMPLE 2C
<p>
<img src="https://i.imgur.com/cEW8nAR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Select the “Networking” tab towards the top of the page and view EXAMPLE 2D inputs to match. 
  
</p>
<br />

EXAMPLE 2D
<p>
<img src="https://i.imgur.com/y6N0A8P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

NEXT: At the Virtual Machine we find that the IP to the Virtual Machine is “4.232.128.178”. See EXAMPLE 2E

EXAMPLE 2E

<p>
<img src="https://i.imgur.com/TCYI48a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


STEP 3 – Log Into the VM and Find IP Address
<p>
Now that we have set up the Virtual Machine we will connecting to it using the application “Windows App” (EXAMPLE 3A) and input the IP address for the VM that we located in EXAMPLE 2E and then input the set credentials we set when creating the VM (see EXAMPLE 3B). Once logged in, we will open the web browser and again look up www.showmyip.com (EXAMPLE 3C).

  
</p>
<br />
EXAMPLE 3A
<p>
<img src="https://i.imgur.com/p1Qa1P7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
</p>
<br />

EXAMPLE 3B
<p>
<img src="https://i.imgur.com/eFVnHNH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

When we look up the IP address for this VM through www.showmyip.com we see that this VM is showing the location for Italy (EXAMPLE 3C).
  
</p>
<br />

EXAMPLE 3C
<p>
<img src="https://i.imgur.com/VHzRzSP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

STEP 4 – CONNECTING TO VPN (Free Version)

Using the local computer go to protonvpn.com and create a free account (if you use the VM then Italian will display on your browser, so use local computer desktop). Once you are logged into your account, copy the URL from the Proton VPN website (EXAMPLE 4A) and then paste the URL to the VM web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>
<img src="https://i.imgur.com/PYiumpH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. See EXAMPLE 4B when this steps are completed.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img src="https://i.imgur.com/wq65Syk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in Netherlands. See EXAMPLE 4C
  
</p>
<br />

EXAMPLE 4C
<p>
<img src="https://i.imgur.com/XZd4J7r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to Netherlands. The website www.showmyip.com shows yet another IP address using the VPN from Netherlands. This is quite amazing.
  
</p>
<br />

EXAMPLE 4D
<p>
<img src="https://i.imgur.com/7ASNQZE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 74.66.243.179
Virtual Machine IP (Italy): 4.232.128.178
Virtual Machine IP VPN (Netherlands) 169.150.196.144

  
</p>
<br />
If you no longer need the VM, ensure to remove it from the Asure account for unwanted charges.

END OF TUTORIAL
