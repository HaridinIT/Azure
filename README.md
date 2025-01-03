<h1>Azure Virtual Networking Infrastructure</h1>

<h2>Description</h2>
In this project, Azure Network Security Groups(NSGs) and Application Security Groups(ASGs) were configured to enhance virtual machine security. NSGs were configured to control inbound and outbound traffic with specific ports and protocols, while ASGs simplified management by logically grouping VMs for rule application. Together, they provide scalable, efficient, and secure network communication.
<br />
<p align="center">
<img src="https://user-images.githubusercontent.com/91347931/157526438-6da4f68b-db88-4931-a041-8474e66d3fe5.png" height="85%" width="85%" alt="Network and Application Security Groups Diagram"/>
</p>

<h2>Languages and Environments Used (PaaS Components) </h2>

- <b>Command Prompt</b> 
- <b>Azure VMs</b>
- <b>Windows Server</b>
- <b>Azure Virtual Network<b>

<h2>Project walk-through:</h2>

<p align="center">
Create and configure Virtual Network: <br/>
<img src="https://imgur.com/AKx1mBV.png" height="80%" width="80%" alt="Virtual Network"/>
<br />
<br />
Create and configure two Application Security Groups  <br/>
<img src="https://imgur.com/p3And6O.png" height="80%" width="80%" alt="Application Security Group 1"/>
<img src="https://imgur.com/foOKBEQ.png" height="80%" width="80%" alt="Application Security Group 2"/>
<br />
<br />
Create Network Security Group and associate to Subnet: <br/>
<img src="https://imgur.com/S2pQZWN.png" height="80%" width="80%" alt="NSG"/>
<img src="https://imgur.com/VFr4HiI.png" height="80%" width="80%" alt="Associate to Subnet"/>  
 
<br />
<br />
Inbound NSG Security Rules :  <br/>
<img src="https://imgur.com/W2Mvo00.png" height="80%" width="80%" alt="Inbound NSG Security Rules"/>
<img src="https://imgur.com/6DNFZ95.png" height="80%" width="80%" alt="Inbound NSG Security Rules"/>
<img src="https://imgur.com/kPcM7OR.png" height="80%" width="80%" alt="Inbound NSG Security Rules"/>
<br />
<br />
Create two VMs and associate VMs to ASGs:  <br/>
<img src="https://imgur.com/p3And6O.png" height="80%" width="80%" alt="Application Security Group 1"/>
<img src="https://imgur.com/foOKBEQ.png" height="80%" width="80%" alt="Application Security Group 2"/>
<br />
<br />
Install IIS on Windows Server:  <br/>
<img src="https://imgur.com/dsEXAYw.png" height="80%" width="80%" alt="Install IIS on VM"/>
<br />
<br />
Verification:  <br/>
<img src="https://imgur.com/0ectexl.png" height="80%" width="80%" alt="Azure VM Public IP"/>
<img src="https://imgur.com/drT2Vck.png" height="80%" width="80%" alt="IIS viewed for Azure VM Public IP"/>
</p>

<h2>Conclusion</h2>
Browser page displayed default IIs welcome page because port 80 is allowed from the internet based on the configuratrion settings of the myAsgwebservers ASG. Therefore, NSG and ASG configurations are working and traffic is being correctly managed.
<br />
