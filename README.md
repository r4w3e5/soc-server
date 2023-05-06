# SOC-Server
### Security operation center:

🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳

✅ SSH protection 22/tcp

✅ HTTP protection 80/tcp

✅ HTTPS protection 443/tcp

✅ NX protection 4000/tcp

✅ Protection against port scanners

✅ SYN-flood protection

✅ Ping of death protection

🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳🔳

1. Install requirements:

```
sudo apt update && sudo apt install curl apache2 apache2-utils iptables -y
```

2. Presetting:

Activate autoloading services:
```
sudo systemctl enable iptables.service
```
```
sudo systemctl enable apache2.service
```

Issue rights to execute:
```
sudo chmod +x /path/to/file/SOC-Server.101
```

Setting up rc-local:
```
sudo systemctl edit --full rc-local
```
```
sudo systemctl enable rc-local
```
```
sudo chmod u+x /etc/rc.local
```

Edit the rc.local configuration settings:
```
sudo nano /etc/rc.local
```

Specify start-up file locations:
```
bash /path/to/file/SOC-Server.101 &
```

### Example:
![изображение](https://user-images.githubusercontent.com/37213906/236634159-76277acf-c0bb-4651-a87a-3de6846f2e39.png)
