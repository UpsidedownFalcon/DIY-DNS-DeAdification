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

--- 

## SSH into VM 

1) Open a termainal e.g command prompt
2) SSH command
```bash
ssh diy-dns-deadification@diy-dns-deadification
```

3) Add fingerprint if prompted
4) Enter password
5) Et voila

--- 

## Update Packages 

```bash
sudo apt update
sudo apt upgrade
```

--- 

## Installing Pi-hole 

[Pi-hole's website](https://pi-hole.net/) leads to its [GitHub repo](https://github.com/pi-hole/pi-hole/#one-step-automated-install) for installation - from which, to install Pi-hole: 

1) Quick install 
```bash
curl -sSL https://install.pi-hole.net | bash
```
2) Static IP assigned later! Continue the installation without static IP for now
3) Use **Cloudflare (DNSSEC)** upstream DNS provider
4) **Yes** to using third party lists for ad blocking 


