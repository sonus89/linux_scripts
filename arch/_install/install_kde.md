Install the bare minimum KDE

    pacman -S xorg plasma-desktop plasma-wayland-session sddm
  
Enable Display Manager & NetworkManager

    systemctl enable sddm

Install very important packages

    pacman -S plasma-nm plasma-pa konsole spectacle firefox