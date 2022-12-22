# DOH Cloudflared Installer For Ubuntu 22.04 Server

Cloudflare DOH server installation for Ubuntu 22.04

### Install
```bash
bash -c "$(curl -L https://raw.githubusercontent.com/azadrahorg/dohCloudflared/main/dohCloudflared.sh)"
```
### How to Manage
Start the service.
```
systemctl start cloudflared
```
View the status of the service.
```
systemctl status cloudflared
```
Restart the service.
```
systemctl restart cloudflared
```
Enable service.
```
systemctl enable cloudflared
```
Disable service.
```
systemctl disable cloudflared
```

### How to test DNS:
Run This Comamnd
```
kdig google.com | grep 127.0.0.1
```
The output should be like below
```
From 127.0.0.1@53(UDP) in 0.2 ms
```

