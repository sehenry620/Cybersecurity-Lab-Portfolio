# Lab Title: Metasploit Backdoor Exploitation

**Date:** [07-01-25]  
**Objective:** Practice generating and deploying a backdoor payload using Metasploit Framework to gain remote access to a Windows 10 target machine.

**Tools Used:**  
- Metasploit Framework  
- Kali Linux  
- Windows 10 (victim machine)  
- msfvenom  
- netcat  

## Lab Overview

This lab involved creating a Windows executable backdoor using `msfvenom`, then delivering it to a victim Windows 10 machine. The goal was to establish a Meterpreter session to remotely control the victim system and practice post-exploitation commands.

## Methodology

1. Generated a reverse TCP payload using `msfvenom` specifying LHOST and LPORT.  
2. Started the Metasploit multi-handler to listen for incoming connections on the specified port.  
3. Transferred the backdoor executable to the victim Windows machine via USB drive.  
4. Executed the backdoor on the victim machine to initiate a connection back to the attacker.  
5. Once the Meterpreter session was established, ran commands to gather system information and take screenshots.

## Results

- Successfully generated and executed the backdoor payload.  
- Established a Meterpreter session with the Windows 10 target machine.  
- Performed basic post-exploitation tasks demonstrating control over the system.

## Lessons Learned

- Gained practical experience with Metasploit payload creation and listener setup.  
- Understood the process attackers use to maintain remote access.  
- Recognized the importance of defensive measures to detect and prevent backdoor infections.

## References

- [Metasploit Unleashed - Payloads](https://www.offensive-security.com/metasploit-unleashed/)  
- [Kali Linux Documentation - msfvenom](https://docs.kali.org/tools/msfvenom)
