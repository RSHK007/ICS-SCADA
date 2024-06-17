# ICS-SCADA

<h1>Module-1 - introduction to ICS/SCADA network defense</h1>
<html>
<body>Security model: <br>
1)authentication -- impersonation, masquerade attacks <br> 
2)confidentiality -- evasdropping <br>
3)integrity -- data tampering <br>
4)availability -- DOS, DDOs<br>

</br>
Authorization: access control purpose <br>
windows : SID (security identifier) <br>
UNIX: Uid  (User Identifier) <br>
</br>
<b> Different types of access control </b>
1)DAC: Discretionary access control -- concept of different user with different privileges </br>
2)MAC: Mandatory access control -- Higher level of protection is avaiable where a owner cannot also change the permissions </br>
3)RBAC: Role based access control -- user is granted a higher level privilege to accomplish a task </br>

</body>


Purdue model

LEVEL-5-Enterprise zone: This where supply chain is managed. OT systems are not directly connected to this level. It collects the data from below level. </br>
LEVEL-4- This is level is for the IT systems of the local plan. It takes orders from level-5 and manages below levels  </br>
ICS-demilittarized zone: This is the layer for sharing information from IT and OT. It is secured as per the standards NIST800-82, NERCIP, ISA 62443 etc.. </br>
LEVEL-3 - site manufacturing and operation control: This is the layer that contains SCADA supervision control. Mainly involves in  operation-level interaction with the systems. </br>
LEVEL- 2- Area supervisory control: this level is where process cell or line-level functions primarily exist
for local control over individual areas of a process </br>
LEVEL 1 - BASIC control: This level compromises what is known as the Basic Process Control Systems, or BPCSs. BPCS is a generic term applying to non-safety-related control systems </br>
LEVEL 0 - process: equipment under control. Physical euipment controlled by level-1 are located here. These include drives, motors, valves, and sensors other components that comprise the actual process </br>


PLCs were invented by Dick Morley in 1964</br>
Ladder logic is the PLC programming language </br>
The people or the organization that sets the standards for ladder logic is PLCOpen. This simply means that ladder logic is described in a standard. That standard is called IEC 61131-3 </br>

Four typical security postures</br>
1)deny all (paranoid)</br>
2)allow all (promiscuous)</br>
3)deny the things i know (permissive)</br>
4)Allow the things i know (prudent)</br>

Prudent approach is followed in most cases </br>

Risk is exposure to the chance of damage or loss</br>
RISK= severity*threat*value </br>
• Severity: maximum impact of an exploited vulnerability</br>
• Threat: likelihood of being attacked </br>
• Value: cost of loss if compromised</br>

Two types of risk:
</br>
1)risk appetite
</br>
Company cannot accept any risk 
</br>
2)risk tolerance 
</br>
Company can accept risk upto certain point
</br>

Two factors to mitigate risk:</br>    
1)policies and procedures -- ask user not to do it</br>
2)Technology -- It enforces user to follow policies </br>

Residual risk - carrying the risk </br>

ICS SCADA generations</br>
1)first generation - monolithic</br>
2)Second generation - distributed</br>
3)Third generation - Networked</br>
4)fourth generation - Cloud</br>

**Threat** -  A threat is any circumstance or event with the potential to adversely impact organizational operations (including mission, functions, image, or reputation), organizational assets, individuals, other organizations, or the Nation through an information system via unauthorized access, destruction, disclosure, modification of information, and/or denial of service</br>

**Threat source** - Threats have some intent or method that may exploit a vulnerability through either intentional or unintentional means, this intent or method is referred to as the threat source</br>

**Vulnerability** -  A vulnerability is a weakness in an information system (including an ICS), system security procedures, internal controls, or implementation that could be exploited or triggered by a threat source</br>

**Threat event** - A threat event is an event or situation that has the potential for causing undesirable consequences or impact</br>

Predisposing conditions are properties of the organization, mission/business process, architecture, or information systems that contribute to the likelihood of a threat event </br>

SP 800-53 contains a taxonomy of security controls, or countermeasures, to mitigate vulnerabilities and predisposing conditions</br>


**MODBUS -502**: The Modbus packet frame can be broken down into two sections: the Application Data Unit (ADU) and the Protocol Data Unit (PDU). The ADU consists of the Address, PDU, and an Error Checking method. The PDU is composed of the function code and the data sections of the Modbus frame.</br>

**Ethernet/IP** : etherNet/IP is more modern than Modbus, it still has security issues that leave the protocol open to attack. EtherNet/IP is typically found running over TCP and UDP ports 44818. However, there is another port that EtherNet/IP utilizes—TCP and UDP port 2222. The reason for this port is that EtherNet/IP has implemented implicit and explicit messaging.</br>

**DNP3**:  DNP3 is typically found on the standard TCP port 20000</br>

PLC7 (S7) attacked by struxnet worm</br>

 BACnet is an ASHARE standard, number 135.1, and is maintained by ASHARE. The BACnet protocol has defined services that allow building devices to communicate with each other
</br>


SCADA/ICS Risk Assessment Process includes three (3) stages</br>
1)Asset Identification and System Characterization </br>
2)Vulnerability Identification and Threat Modelling </br>
3)Risk Calculation and Management</br>


LAB-1
tcp.flags.syn==1 & tcp.flags.ack==1
tcp.flags.push==1


<h1>Module-2 - TCP/IP-101</h1>

internet started in 1987. 
internet protocols 
1)IP
2)TCP
3)UDP

client runs on ports greater than 1023 -ephemeral 
servers runs on ports less than 1023 -- privileged

TCP - connection oriented. we get acknowledge for data received
UDP - connectionless. No data tramission gurentee 

Each packet is encapsulted with the header as it goes down and decapsulates on the server side to reach application layer
encapsulation --
deencapsultion -- 

TCP/IP - Department of defense </br>

switch are layer 2 devices</br>
routers are layer 3 devices</br>
802.3 ethernet and 802.5 tokenring</br>
protocol analysis tools</br>
1)wireshark</br>
2)omnipeek</br>
3)sniffer</br>



</html>

