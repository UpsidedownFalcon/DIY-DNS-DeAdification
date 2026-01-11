# DIY-DNS-DeAdification
Pi-hole based DNS server for network wide ad blocking 

---

## VM Creation 

1) Logged into ProxMox on port 8006
2) Created a new VM with
- **ubuntu-22.04.5-live-server-amd64.iso** (LTS)
- **VirtIO SCSI Single** SCSI controller
- **Quemu Agent** enabled
- **32GiB** disk size
- **1 socket** with **2 cores**
- **2048MiB** of memory

<img width="666" height="491" alt="image" src="https://github.com/user-attachments/assets/a09a5eb1-bef1-4b98-b647-d2b5d43113fa" /> 

--- 

## Ubuntu Bios 

1) Added the following server information: 
- **Your name:** diy-dns-deadification
- **Your server's name:** diy-dns-deadification
- **Username:** diy-dns-deadification
- **Password:** diy-dns-deadification [TEMPORARY]

2) Installed SSH


