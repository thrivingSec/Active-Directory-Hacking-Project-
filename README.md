# Active Directory Home Lab Network Hacking

## Objective
Understand the basics of Active Directory and setup a home lab Active Directory network consisting of a domain controller(windows 2019 server) and two workstations(windows 10 enterprise) connected to the domain and a attacker's machine(kali Linux). 

Understand and describe all the possible attack scenarios. Dig deep into the technical stuff like protocols, tools used to exploit, features etc. 

Enumerate the network and execute the attacks and make a well documented report.

Learn about the post compromise enumeration and exploitation and execute it. Make a well documented report of the same.

Study about the defense mechanism to make AD in an enterprise environment more secure against the possible attacks.


### Skills Learned

- Mastered Active Directory fundamentals through setting a home lab network.
- Gained expertise in AD domain network attack vectors LLMNR poisoning, SMB relay, compromising ipv4 networks using ipv6 attacks with Responder and ntlmrelayx, mitm6 for initial access.
- Developed advanced post compromise enumeration skills using tools like PowerView and BloodHound.
- Developed advanced post-compromise exploitation skills including pass-the-hash/pass-the-passwordand Kerberoasting using impacket toolkit
- Performed high-level attack simulations like token impersonation and golden ticket attacks to get domain admin access and unlimited access on the domain network
- Authored detailed incident reports documenting attack methodologies, tools used, and mitigation strategies to enhance organizational security posture.

### Tools Used
Initial Attack Tools: responder, ntlmrelayx.py, mitm6, (metasploit, psexec, wmiexec, smbexec)
	
Post Compromise Enumeration: PowerView, Bloodhound
			
Post Compromise Attack Tools: crackmapexec, sercretsdump.py, psexec, metasploit, GetUserSPNs.py, mimikatz

### Home Lab AD Network Setup Topology
Domain Name: BiriyaniBlend.trio

**COMPUTERS**

Domain Controller: Coral401-DC(coral401-DC.BiriyaniBlend.trio)

Domain Controller IP: 10.0.2.6

Workstation1:

Machine Name: BLENDTESTER(BLENDTESTER.BiriyaniBlend.trio)

IP: 10.0.2.7

Workstation2:

Machine Name: BLENDTS(BLENDTS.BiriyaniBlend.trio)

IP: 10.0.2.15

**USERS**

DOMAINUSERS:

Avneet Kaur: Local Admin at workstation1:(SAM Folder Name: akaur): (akaur@BiriyaniBlend.trio)

Tushar Shaw: Local Admin at workstation1 and workstation2: (SAM Folder Name: tshaw): (tshaw@BiriyaniBlend.trio)

ADMINISTRATOR: DOMAIN ADMIN

LOCALUSERS:

Avneet Kaur: Workstation1

Tushar Shaw: Workstation2
