#!/bin/bash
cd
if [ $(id -u) != 0 ]
then
echo "Ejecute el script como root"
exit
fi
echo -e "\033[1;30mInstalando...\033[0m"
mkdir /etc/VpsPackdir 2>/dev/null
mkdir /etc/VpsPackdir/limite 2>/dev/null
mkdir /etc/VpsPackdir/senha 2>/dev/null
rm -rf /bin/limite 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/limite > /bin/limite
chmod +x /bin/limite
rm -rf /bin/criarusuario 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/criarusuario > /bin/criarusuario
chmod +x /bin/criarusuario
rm -rf /bin/deletarusuario 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/deletarusuario > /bin/deletarusuario
chmod +x /bin/deletarusuario
rm -rf /bin/redefinirusuario 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/redefinirusuario > /bin/redefinirusuario
chmod +x /bin/redefinirusuario
rm -rf /bin/vpspack 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/vpspack > /bin/vpspack
chmod +x /bin/vpspack
rm -rf /bin/speedtest.py 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/speedtest.py > /bin/speedtest.py
chmod +x /bin/speedtest.py
rm -rf /bin/dropbear 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/dropbear > /root/dropbear
chmod +x /root/dropbear
rm -rf /bin/shadowsocks 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/shadowsocks > /bin/shadowsocks
chmod +x /bin/shadowsocks
rm -rf /bin/banner 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/banner > /bin/banner
chmod +x /bin/banner
rm -rf badvpn 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/badvpn > badvpn
chmod +x badvpn
rm -rf /bin/menu_firewall 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/menu_firewall > /bin/menu_firewall
chmod +x /bin/menu_firewall
m -rf /bin/menu_hosts 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/menu_hosts > /bin/menu_hosts
chmod +x /bin/menu_hosts
m -rf /bin/menu_shadowsocks 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/menu_shadowsocks > /bin/menu_shadowsocks
chmod +x /bin/menu_shadowsocks
m -rf /bin/menu_badvpn 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/menu_badvpn > /bin/menu_badvpn
chmod +x /bin/menu_badvpn
m -rf /bin/menu_backup 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/menu_backup > /bin/menu_backup
chmod +x /bin/menu_backup
rm -rf /bin/webmin 2>/dev/null
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/webmin > /bin/webmin
chmod +x /bin/webmin
wget -o /dev/null -O- https://raw.githubusercontent.com/AizenNetFreeMx/vpsmanager/master/stunnel.sh > /bin/stunnel
chmod +x /bin/stunnel
clear
echo "alias @actualiza='wget https://raw.githubusercontent.com/diesel09/mx2/master/install && bash install'" >> .bashrc
echo -e "\033[1;32mInstalacion Finalizada\n\033[1;37mEjecute:"
echo -e "\n\033[1;32mvpspack \033[1;37mMenu de opciones"
echo -e "\033[1;32mOpcion 3 \033[1;37mCrear un usuario con fecha y limite"
echo -e "\033[1;32mScript Oficial por: \033[1;37mFelipe Couoh: NetFree Mx"
echo -e "\033[1;32mInstalada \033[1;37mVersion 3.0"
rm -rf install
