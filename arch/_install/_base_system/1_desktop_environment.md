# Desktop Environment - Basic Installation Guide

## Install & Customize KDE

Install the Bare Minimum for KDE

    pacman -S xorg xorg-server xorg-xinit plasma-desktop sddm
  
Enable Display Manager & NetworkManager

    systemctl enable sddm
    systemctl enable NetworkManager

Install very important packages

    pacman -S dolphin konsole plasma-nm plasma-pa packagekit-qt6 discover kscreen gwenview gedit firefox spectacle ktorrent ark p7zip unrar
    reboot
  
Setup Bluetooth

    pacman -S bluez bluez-utils bluedevil
    systemctl enable bluetooth

Unchroot and reboot

    exit
    reboot

Customize Look and Feel

- Firefox -> Settings -> General -> Dark
- System Settings
    - Appearance -> Global Theme -> Get New -> Download a Theme ( i.e. Utterly Sweet ) -> Apply it in Global Themes
    - Global Theme -> Night Light
    - Window Management -> Desktop Effects -> Select the followings:
        - Magic Lamp
        - Blur
- Konsole -> Settings -> Configure Konsole -> Profiles -> New -> OK -> Select new Profile -> Set as Default -> Edit -> Appearance -> Get New -> Select Color Scheme ( i.e. Utterly Sweet ) -> Install & Apply 

Add Hotkey for Screenshot

    1. Open Spectacle
    2. Select: Configure -> Shortcuts
    3. Add Win+Shift+S as Capture Rectangular Region

Install yay Package Manager

    git clone https://aur.archlinux.org/yay.git
    cd yay
    makepkg -si

