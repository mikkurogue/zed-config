# Mikkurogue's Zed settings

This is just my zed settings and config I use for my Zed editor.

Currently its kind of barren but I plan on expanding this along side Zed when it receives more updates.


## Zed on Arch Linux with Hyprland:

Follow below to use dolphin and kde (inside hyprland)

https://wiki.archlinux.org/title/XDG_Desktop_Portal#Force_desktop_environment

you simply have to do these:

    sudo pacman -S xdg-desktop-portal-kde
    create ~/.config/systemd/user/xdg-desktop-portal.service.d/override.conf file and add

[Service]
Environment="XDG_CURRENT_DESKTOP=KDE"

to it

    systemctl --user deamon-reload
    systemctl --user restart xdg-desktop-portal
