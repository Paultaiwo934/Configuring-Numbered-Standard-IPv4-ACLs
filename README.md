<h1>Configured Numbered Standard IPv4 ACLs</h1>

<h2>Description</h2>
This project focuses on defining filtering criteria, configuring standard access control lists (ACLs), applying ACLs to router interfaces, and verifying and testing the ACL implementation. ACLs are router configuration scripts that control whether a router permits or denies packets based on the source address.<br />


<h2>Languages and Utilities Used</h2>

- <b>CLI</b> 


<h2>Environments Used </h2>

- <b>CISCO Packet Tracer</b> 

<h2>Program walk-through:</h2>

- <b>Topology: <b/> 
<br/>
<img src="https://imgur.com/UlQrXaj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

<br/>
Step 1: Tested network connectivity by pinging other devices on the network. Ping was suscessful:
<br/>
<img src="https://imgur.com/UY0TnUa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />Step 2: Created an ACL using the number 1 on R2 with a statement that denies access to the 192.168.20.0/24 network from the 192.168.11.0/24 network, then applied the ACL by placing it for outbound traffic on the GigabitEthernet 0/0 interface: <br/>
<img src="https://imgur.com/dxgzvpv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />Step 3: Created an ACL using the number 1 on R3 with a statement that denies access to the 192.168.30.0/24 network from the PC1 (192.168.10.0/24) network, then applied the ACL by placing it for outbound traffic on the GigabitEthernet 0/0 interface:  <br/>
<img src="https://imgur.com/xs2guQK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 4: Verified ACL configuration and functionality using "Show Running Config". Ping failed for networks with ACL configured.
  <br/>
<img src="https://imgur.com/iAiSjyY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>
<img src="https://imgur.com/yVuwKaq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<img src="https://imgur.com/BuyvNqL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
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
