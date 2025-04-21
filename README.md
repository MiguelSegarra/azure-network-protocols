<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com) [ Coming Soon! ]

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

### Step 1: Deploy and Connect Azure Virtual Machines

- Deploy one **Windows 10 VM** and one **Ubuntu Server 20.04 VM**.
- Ensure both VMs are on the same virtual network and subnet.
- Connect to the Windows VM using RDP.

### Step 2: Install Wireshark and Capture Traffic

- Install **Wireshark** on the Windows VM.
- Begin capturing network packets on the primary interface.
- Observe background traffic and identify common protocols (DNS, ICMP, etc.).

### Step 3: Generate and Inspect Traffic Between VMs

- Use tools like `ping`, `curl`, `ssh`, and `telnet` from one VM to the other.
- Watch how this traffic appears in Wireshark.
- Analyze packet details, source/destination IPs, and protocols.

### Step 4: Modify and Test Network Security Groups (NSGs)

- Apply NSG rules to block/allow specific types of traffic (e.g., block ICMP, allow SSH).
- Re-run tests to verify which traffic is allowed or denied.
- Observe real-time effects of NSGs on traffic visibility and flow in Wireshark.

