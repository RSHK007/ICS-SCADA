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




</br>


</html>

