# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:
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
<img width="1466" height="1056" alt="Screenshot 2025-09-22 145215" src="https://github.com/user-attachments/assets/3b9fa840-e5bd-4d11-a60a-741b78179342" />

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
•	PDU details for local communication<br>
  At 172.16.31.2
  <img width="1917" height="1083" alt="Screenshot 2025-09-22 135802" src="https://github.com/user-attachments/assets/0623091b-6ada-4381-a05d-792877e780bc" />
  At 172.16.31.3
  <img width="1457" height="1046" alt="Screenshot 2025-09-22 142629" src="https://github.com/user-attachments/assets/5f07c273-5f3c-4ba9-93b7-b39460915ce5" />
  At 172.16.31.4
  <img width="1919" height="1053" alt="Screenshot 2025-09-22 142914" src="https://github.com/user-attachments/assets/c94a3c9e-1ed3-4537-b9d8-4769fd35de90" />

•	PDU details for remote communication<br>
At 10.10.10.2
<img width="1463" height="1053" alt="Screenshot 2025-09-22 143341" src="https://github.com/user-attachments/assets/8c52f5f4-aa2c-4cdf-90fa-c21898a688e7" />

•	Tables showing MAC/IP changes through each device<br>
For Local Network Communication
<img width="1459" height="1045" alt="Screenshot 2025-09-22 144116" src="https://github.com/user-attachments/assets/7fbd398d-5135-4de4-826c-b48caf38b9d0" />
For Remote Network Communication
<img width="1457" height="1047" alt="Screenshot 2025-09-22 144318" src="https://github.com/user-attachments/assets/16f45709-7976-477d-aabd-9ac795d325ac" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

