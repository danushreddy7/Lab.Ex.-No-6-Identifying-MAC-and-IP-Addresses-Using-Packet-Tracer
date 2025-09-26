# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:13-09-2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication:
<img width="1920" height="1080" alt="491366719-e2d95ecd-345a-43c4-9041-3afa991d7343" src="https://github.com/user-attachments/assets/f08c0b07-8b6a-45d4-b4eb-9691081abd14" />
<img width="1920" height="1080" alt="491366714-4208635d-8b3b-4800-bea7-cb6b9e1068de" src="https://github.com/user-attachments/assets/0f4afb48-750b-4607-bde3-231a2b78d696" />
<img width="1920" height="1080" alt="491366707-b07c6fe5-81c6-4cb6-90e1-b90ba4515f35" src="https://github.com/user-attachments/assets/f8d02104-ca3e-481c-9487-69bfaea8dbed" />
<img width="1920" height="1080" alt="491366686-c4e990a1-1058-408c-9269-cb0a87fc0116" src="https://github.com/user-attachments/assets/61b99edb-7ec9-42c9-a673-548fbdcd326a" />

This shows the configruation of the PDU for local communication.


•	PDU details for remote communication:
<img width="1920" height="1080" alt="491367487-32cb3b36-63b0-4c16-a6c8-99deabfebd0b" src="https://github.com/user-attachments/assets/2e9a09db-90ee-4bed-a670-6e3f6df2a145" />
<img width="1920" height="1080" alt="491367480-cb4c88fb-ff42-4d38-9dde-4868ca824fea" src="https://github.com/user-attachments/assets/cb9a2e14-a4ff-4d3e-baf1-54d38f64d33f" />
<img width="1920" height="1080" alt="491367464-5a36660d-e0bc-4c84-82f5-afb39b6a068f" src="https://github.com/user-attachments/assets/51c66efd-3686-4633-9c46-108d292fbadf" />
<img width="1920" height="1080" alt="491367624-d98c44ca-018a-4ac0-b6b4-230c3ffbfe6e" src="https://github.com/user-attachments/assets/d941a2b5-8852-4273-8ba9-b78c253c952b" />
<img width="1920" height="1080" alt="491367609-74f8cfe3-b101-4c1b-9ba2-bb7773c5912e" src="https://github.com/user-attachments/assets/4374ca4b-1c53-4c8e-b072-807e3f8025f4" />
<img width="1920" height="1080" alt="491367595-1fa11d1b-824e-4176-a8a1-3d58bccc18c0" src="https://github.com/user-attachments/assets/5c06dae8-f829-4c0b-b530-a925382b2013" />

The above figures shows a clear detail of PDU for remote communication.

•	Tables showing MAC/IP changes through each device:

<img width="1920" height="1080" alt="491367656-307d7d21-5df7-47ef-8468-76971ac72b6a" src="https://github.com/user-attachments/assets/7221339c-44f0-4208-8721-ccee8640fa61" />
<img width="1920" height="1080" alt="491367648-75f91671-9be1-4ef9-83e7-ca6976bc1cf3" src="https://github.com/user-attachments/assets/feffdced-8d3d-46ec-b2d8-3d093574ba75" />

___________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

