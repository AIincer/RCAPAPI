# dnsmasq einrichten
installieren
```
sudo apt update
sudo apt install dnsmasq -y
```
konfig backup + edt
```
sudo cp /etc/dnsmasq.conf /etc/dnsmasq.conf.bak
sudo nano /etc/dnsmasq.conf
```
autostart
```
sudo systemctl enable dnsmasq
sudo systemctl start dnsmasq
```
# Router verbinden
```Heimnetz → Netzwerk → Netzwerkeinstellungen```
```
Bevorzugter DNS: <server-ip>
Alternativer DNS: 1.1.1.1 (optional)
```
