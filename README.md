<p align="center">
<img width="418" height="120" alt="Azure Logo" src="https://github.com/user-attachments/assets/3b6347a2-5104-4eb2-b4a2-0a7a28524ee0" />
</p>

<h1>Common Networking Commands</h1>
Trouble shooting network issues is very common in IT work. Network commands are a very important tools you should know how to use in order to trouble shoot network issues effectively. 
In this tutorial I will show you how to use 3 very common Network commands: 

- Ping 
- Nslookup 
- Ipconfig

We will explore how to use these commands in the Windows virtual machine from the last tutorial.

<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Powershell

<h2>Operating Systems Used </h2>

- Windows 11

<h2>High-Level Steps</h2>

- Log in to our Windows VM from the last tutorial 
- Open powershell
- Run common networking commands and see how they work

<h2>Commands</h2>

<p>
<img width="1117" height="632" alt="Snapshot#35" src="https://github.com/user-attachments/assets/a34d00f0-8c59-4b89-8075-514d3a448d3f" />
</p>
<p>
First, is the ping command. Type "ping" followed by an IP address. This will send 4 ICMP packets to that IP address. If the packets are able to reach the IP before their TTL expires, that means our computer is able to connect to that machine. This is used as a diagnostic tool when trouble shooting to establish if our computer is even able to connect to the other machine. 

You can try it with domain names, because after all domain names are just IP addresses made human readable. 
</p>
<br />

<p>
<img width="1126" height="639" alt="Snapshot#36" src="https://github.com/user-attachments/assets/a6fdecdf-0214-4ce5-9e5a-c7c2126c9fa2" />
</p>
<p>
Speaking of domain names, you can look up the IP address of a domain name with nslookup. Type the command "nslookup" followed by a domain name. This will give you the IP address that domain name resolves to. Here's a good example of using this command for troubleshooting network issues. Imagine you can't connect to a certain website. You can get the IP address of the website's domain name using nslookup. You can take that IP address and use the ping command to see if you are able to connect to the website's server. If you are able to connect to the server using ping, but not able to connect to it with the domain name, that can point to your computer not  resolving the domain name to the correct IP address anymore. You can fix that with our last command, which is ipconfig.
</p>
<br />

<p>
<img width="1123" height="640" alt="Snapshot#37" src="https://github.com/user-attachments/assets/fd644768-6cf0-408f-91d6-d58fccb032e0" />
<img width="1123" height="635" alt="Snapshot#38" src="https://github.com/user-attachments/assets/271c80e3-ba7c-4017-9d24-b2c382f7c6cc" />
<img width="1119" height="635" alt="Snapshot#39" src="https://github.com/user-attachments/assets/bb93d68e-999e-4e99-af84-32815ef7938b" />
</p>
<p>
ipconfig allows you to view the networking configurations of your computer. Simply type in "ipconfig" and it will give you list of networking configurations. You can see what IP address you are using, what subnet mask you are using, what is your default gateway, etc.

This isn not really a complete list though. "ipconfig /all" will give you a much more detailed list. You can see what DNS servers you are using, what DHCP servers you are using, when your DHCP lease expires and much more.

In regards to that troubleshooting example I brought up talking about the nsllokup command, this is how you can use ipconfig to fix it. What will happen is sometimes our DNS cache will be outdated and our computer 
will reslove domain names to the wrong IP address. To reset our DNS cache, we can use the command "ipconfig /flushdns". This will clear our DNS cache, so next time we type in that website's domain name, our comupter will be forced to get the updated IP address from it's DNS server.

There is much more you can do with ipconfig, but this is just scratching the surface.
</p>
<br /> 


<p>
Awesome! You know some very important network commands. This is just streacthing the surface of evrything you can do. You should research more commands to exapnd your tool set.
</p>
<br />
