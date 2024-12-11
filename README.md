# PJPT-notes

### Steps used to gain access to windows 7 ultimate 7601 using [ms17-010 eternalblue](https://www.rapid7.com/db/modules/exploit/windows/smb/ms17_010_eternalblue/)
- nmap -p- -A -T4 172.16.4.129
	- 445/tcp   open  microsoft-ds Windows 7 Ultimate 7601 Service Pack 1 microsoft-ds (workgroup: WORKGROUP)
	- smb2-security-mode: 
		|   2:1:0: 
		|_    Message signing enabled but not required
		|_nbstat: NetBIOS name: WIN-845Q99OO4PP, NetBIOS user: <unknown>, NetBIOS MAC: 00:0c:29:15:5e:86 (VMware)
- search google for vulnerabilities for the specific windows version
- in this case it was ms17-010 eternalblue
- search for vulnerability in metasploit
- first select related auxiliary modules (use _)
- set rhost and run the payload, gained access very easily automatically

