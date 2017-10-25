# INSTALATION-ARCH-LINUX00

instalaçao do arch linux modo grafico anywere

todos os comandos abaixo
#setando rede wireless
pacman -S wireless_tools wpa_supplicant wpa_actiond netcf dialog

systemctl enable net-auto-wireless.service

sudo pacman -S xorg-server xorg-xinit xorg-server-utils 
mesa ttf-dejavu samba smbclient networkmanager 
networkmanager-vpnc networkmanager-pptp 
networkmanager-openconnect network-manager-applet 
gvfs gvfs-smb sshfs chromium firefox vlc leafpad nano

#setar a home
sudo pacman -S xdg-user-dirs
xdg-user-dirs-update


#instalar AUR
sudo leafpad /etc/pacman.conf

#escrever:
[archlinuxfr]
SigLevel = Never
Server = http://repo.archlinux.fr/$arch

sudo pacman -Syy

#checar se tem atualizacoes
sudo pacman -Syu

sudo pacman -S yaourt ttf-liberation
