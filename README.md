<h1>Connecting to a Windows 10 Virtual Machine through Remote Desktop Protocol (RDP)</h1>
This walkthrough shows how to create a Windows 10 Virtual Machine inside Microsoft Azure, deploy it, and then connect to that same Virtual Machine using Remote Desktop Protocol all on a Windows 11 computer. <br />

<h2>Environments and Technologies used</h2>

- Microsoft Azure
- Remote Desktop Protocol

<h2>Operating Systems Used</h2>

- Windows 11 (Local Device)
- Windows 10 (Virtual Machine)

<h2>Creation, Deployment, and Connection Steps</h2>

- Creating a Windows 10 Virtual Machine in Microsoft Azure
- Deploying the Windows 10 Virtual Machine
- Connecting to the Windows 10 Virtual Machine using Remote Desktop Protocol (RDP)

<br />

<h2>Creating and Deploying a Windows 10 Virtual Machine in Microsoft Azure</h2>

<p>
  <img src="https://github.com/user-attachments/assets/bd606dad-e23a-4dea-8340-246a47f074f6" height="80%" width="80%">
</p>
<p>First thing you want to do is open your browser to log into your Microsoft Azure Account/Subscription.</p> <br/>

<p>
  <img src="https://github.com/user-attachments/assets/88502913-a43b-4b56-82e8-107534af76e8" height="80%" width="80%">
</p>
<p>Then in the search bar you want to search "virtual machines". Once you make it to this screen, click on "+ Create" and then click on "Azure virtual machine" in the dropdown box that comes up.</p><br />

<p>
  <img src="https://github.com/user-attachments/assets/2c6e8f95-4ddf-4fb8-bf05-19651c33ce1a" height="80%" width="80%">
</p>
<p>Now under the "Basics" section of this screen we can configure some details to build our Windows 10 VM. For "Resource group" click "Create new" and create a name for your resource group that will be created. Next, for "Virtual machine name" create a name for your VM. Then, make sure your "Region" is selected if it isn't already. Next, scroll down to your "Availability zone" and make sure it has "Zone 1" in the field. Now for the "Image", make sure we select "Windows 10 Pro, version 22H2 - x64 Gen2 (free services eligible)". Now scroll down some more and for the "Size" select "Standard_D2as_v4 - 2 vcpus, 8 GiB memory ($70.08/month)", and if you don't see that option, make sure to find something that has at least 2 vcpus and 8 GiB memory. After that, under "Administrator account" create a Username and Password for your VM (save those credentials for later). Next, under "Inbound port rules" for "Public inbound ports" select "Allow selected ports" and for "Select inbound ports" select "RDP (3389)". And lastly, scroll down to the licensing box and make sure it is checked. Now you can click "Review + create" at the very bottom to create your VM.</p><br />

<p>
  <img src="https://github.com/user-attachments/assets/dbf302ca-8250-4d17-af61-1995e4d92a90" height="80%" width="80%">
</p>
<p>Once you wait a little bit and see the green "Validation passed" banner at the top of the screen click on "Create" at the bottom of the screen to create and deploy your Windows 10 VM.</p><br />


<h2>Connecting to the Windows 10 Virtual Machine using Remote Desktop Protocol (RDP)</h2>

<p>
  <img src="https://github.com/user-attachments/assets/2fb35ee5-4531-43c9-bea0-d1eb7a3db0a0" height="80%" width="80%">
</p>
<p>You should see this screen indicating that the VM deployment is complete. From here you can click "Go to resource" to access you VM resource you just created.</p><br />

<p>
  <img src="https://github.com/user-attachments/assets/2327e743-6912-4326-9adf-059ff37f72a0" height="80%" width="80%">
</p>
<p>Once you get to this screen you are going to want to copy the "Public IP addreess". This is the IP address that we will use to connect to using RDP. At the bottom of the screen in your Windows 11 Operating System search bar search for and open "Remote Desktop Connection".</p><br />

<p>
  <img src="https://github.com/user-attachments/assets/1582c15d-bf34-4469-84a2-36c9c3cea419" height="80%" width="80%">
</p>
<p>Once the Remote Desktop Connection window pops up, input the Public IP address of the Windows 10 VM you just created into the "Computer: " field. Then click "Connect". You will then be asked to enter your credentials. These are the credentials I asked you to create and save when we created the VM in Microsoft Azure. After you enter your credentials click "Okay".</p><br />

<p>
  <img src="https://github.com/user-attachments/assets/e6c6ab24-6275-4af2-a219-3bb850864fa8" height="50%" width="50%">
</p>
<p>When this screen pops up, just click "Yes". Once you click "Yes" you will begin to connect to your Windows 10 VM and you can continue to configure the privacy settings of the VM Operating System upon start up. Now you can start using the Windows 10 VM as if it was an actual Windows 10 device sitting in front of you.</p>
