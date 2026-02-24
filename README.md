<p align="center">
<img width="418" height="120" alt="Azure Logo" src="https://github.com/user-attachments/assets/3b6347a2-5104-4eb2-b4a2-0a7a28524ee0" />
</p>

<h1>Common Networking Commands</h1>
Trouble shooting network issues is very common in IT work. Network commands are a very important tools you should know how to use. 
In this tutorial I will show you how to use 3 very common ones: 

- Ping 
- Nslookup 
- Ipconfig

We will explore these commands in the Windows VM from the last tutorial.

<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Powershell

<h2>Operating Systems Used </h2>

- Windows 11

<h2>High-Level Steps</h2>

- Login to our Windows VM from the last tutorial 
- Open powershell
- Run some common networking commands

<h2>Commands</h2>

<p>
<img width="1117" height="632" alt="Snapshot#35" src="https://github.com/user-attachments/assets/a34d00f0-8c59-4b89-8075-514d3a448d3f" />
</p>
<p>
First is the ping command. Type ping followed by an IP address. This will send 4 signals to that IP. If the signals are able to reach the IP before their TTL expires, that means our computer is able to connect to that machine. This is used as a diagnostic tool when trouble shooting to establish if our computer is even able to connect to the other device. 

You can try it will domain names, because after all domain names are just IP addresses made human readable 
</p>
<br />

<p>
<img width="1126" height="639" alt="Snapshot#36" src="https://github.com/user-attachments/assets/a6fdecdf-0214-4ce5-9e5a-c7c2126c9fa2" />
</p>
<p>
Speaking of domain names, you can look up the IP address of a domain name with nslookup. This can be useful with trouble shooting if you can’t connect to a website, to see if the IP address for that website is still the same 
</p>
<br />

<p>
<img width="1123" height="640" alt="Snapshot#37" src="https://github.com/user-attachments/assets/fd644768-6cf0-408f-91d6-d58fccb032e0" />
<img width="1123" height="635" alt="Snapshot#38" src="https://github.com/user-attachments/assets/271c80e3-ba7c-4017-9d24-b2c382f7c6cc" />
<img width="1119" height="635" alt="Snapshot#39" src="https://github.com/user-attachments/assets/bb93d68e-999e-4e99-af84-32815ef7938b" />
</p>
<p>
Last command is ipconfid, This allows you to view the networking configurations of your computer. 

Ipcongid /all will show more delta 

Ipconfig /lfushdns will clear dns cache 

There is much more you can do, but this is just scratching the surface.
</p>
<br /> 


<p>
Awesome! You know some very important network commands. This is just streacthing the surface of evrything you can do. You should research more commands to exapnd your tool set.
</p>
<br />
