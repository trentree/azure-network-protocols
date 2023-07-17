# azure-network-protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create resources through virtual machine (Windows 10 and Linux)
- Observe ICMP (internet control message protocol) Traffic
- Observe SSH (Secure Shell) Traffic
- Observe DNS (Domain Name System) Traffic
- Observe RDP (Remote Desktop Protocol) Traffic

<h2>Actions and Observations</h2>

<p>
  
![Screenshot 2023-07-17 132033](https://github.com/trentree/azure-network-protocols/assets/129711900/92034b92-1395-490f-8962-f4f032bd83de)

</p>
<p>
First and foremost, our resources are created. VM1 for Windows Operating System and VM2 for Unbuntu Operating System.
</p>
<br />

<p>
  
![Screenshot 2023-07-17 132102](https://github.com/trentree/azure-network-protocols/assets/129711900/4e372066-1505-4945-b4af-b9733138160a)

</p>
<p>
Next, we boot up our VM1 and download Wireshark.
</p>
<br />

<p>
  
![Screenshot 2023-07-17 132213](https://github.com/trentree/azure-network-protocols/assets/129711900/39e9c972-8c89-4aa7-98fc-bd0c54576c58)

</p>
<p>
Once Wireshark is downloaded we type ICMP (Internet control message protocol) into the search bar.
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132305](https://github.com/trentree/azure-network-protocols/assets/129711900/4961f1c0-432e-43a3-9890-2e92fbb35a11)

</p>
<p>
Then we will go to our VM2 and deny our inbound security role.
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132323](https://github.com/trentree/azure-network-protocols/assets/129711900/d548fb26-e6be-4ea0-af07-5c8641ebde72)

</p>
<p>
We visit back to our VM1 and see our PowerShell pings times out the requests.
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132410](https://github.com/trentree/azure-network-protocols/assets/129711900/efc5cf6e-e7d4-476f-81ed-b446ba522a9f)

</p>
<p>
Next, we type in SSH (Secure Shell) into the search bar.
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132459](https://github.com/trentree/azure-network-protocols/assets/129711900/069d4205-d6a0-4ca0-aa78-52d7bee02bb9)

</p>
<p>
Here, we type "TCP port == 22" which allows remote admins access to the VM.
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132544](https://github.com/trentree/azure-network-protocols/assets/129711900/cc231804-b3a7-4d77-9649-6f5bb784966b)

</p>
<p>
"DNS" is typed in the search bar.
</p>
<br />
<p>
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132609](https://github.com/trentree/azure-network-protocols/assets/129711900/90e70ab5-18e6-4a60-8a27-290a65636395)

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
</p>
<br />
<p>
  
![Screenshot 2023-07-17 132653](https://github.com/trentree/azure-network-protocols/assets/129711900/e3848b83-d0e5-41b6-98d0-af539a44fd8f)

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
