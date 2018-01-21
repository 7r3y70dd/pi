# Download: https://www.raspberrypi.org/downloads/raspbian
# Download: https://etcher.io
% touch /Volumes/boot/ssh
% cat << EOF > /Volumes/boot/wpa_supplicant.conf
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
network={
  ssid="[SSID]"
  psk="[PWD}"
  key_mgmt=WPA-PSK
}
EOF
% nmap -p 22 --open -sV 192.168.[X].*
% sudo nmap -sP -PR 192.168.[X].*
% arp-scan -I en0 192.168.X.0/24
