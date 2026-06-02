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
// nach änderung
```
sudo systemctl restart dnsmasq
sudo systemctl enable dnsmasq
```
# Router verbinden
```Heimnetz → Netzwerk → Netzwerkeinstellungen → IP-Adressen → IPv4-Einstellungen → Heimnez```
```
Lokaler DNS-Server: <server-ip>
```
# Reverse Proxy einrichten
installieren
```
sudo apt update
sudo apt install nginx -y
```
starten
```
sudo systemctl enable nginx
sudo systemctl start nginx
```
konfig
```
sudo nano /etc/nginx/sites-available/main-proxy
```
konfig aktiviren
```
sudo rm /etc/nginx/sites-enabled/default
sudo ln -s /etc/nginx/sites-available/main-proxy /etc/nginx/sites-enabled/
```
// neusterten
```
sudo systemctl restart nginx
```
