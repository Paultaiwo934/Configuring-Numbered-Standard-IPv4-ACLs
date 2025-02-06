<h1>Configuring Numbered Standard IPv4 ACLs</h1>

<h2>Description</h2>
This project focuses on defining filtering criteria, configuring standard access control lists (ACLs), applying ACLs to router interfaces, and verifying and testing the ACL implementation. ACLs are router configuration scripts that control whether a router permits or denies packets based on the source address.<br />


<h2>Languages and Utilities Used</h2>

- <b>CLI</b> 


<h2>Environments Used </h2>

- <b>CISCO Packet Tracer</b> 

<h2>Program walk-through:</h2>

- <b>Topology: <b/> 
<br/>
<img src="https://imgur.com/2eVn2GF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

- <b>Enabled port security on F0/1 and F0/2 on the switch and set the maximum devices that can access the ports to one so only PC 1 and PC 2 in our topology can access these ports.
- Secured the ports so that the MAC address of a device is dynamically learned and added to the running configuration.
- Set the violation mode so that the F0/1 and F0/2 are not disabled when a violation occurs, but a notification of the security violation is generated, and packets from the unknown source are dropped.
- Disabled all the remaining unused ports:
<br/>
<img src="https://imgur.com/9k1HCTt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Verify port security is enabled and the MAC addresses of PC1 and PC2 were added to the running configuration: <br/>
<img src="https://imgur.com/RREJ8BA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A Rogue laptop was connected to port F0/2, this was flagged as a violation as only PC2 is allowed to connect to F0/2. Therefore, the rogue laptop could not ping PC1:  <br/>
<img src="https://imgur.com/t8yKBMS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>
<img src="https://imgur.com/qX1P3SC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
