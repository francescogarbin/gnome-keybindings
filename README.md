# Export all keybindings from one PC
dconf dump /org/gnome/desktop/wm/keybindings/ > gnome-keybindings.dconf
dconf dump /org/gnome/settings-daemon/plugins/media-keys/ > media-keys.dconf

# Import all keybindings on the other PC
dconf load /org/gnome/desktop/wm/keybindings/ < gnome-keybindings.dconf
dconf load /org/gnome/settings-daemon/plugins/media-keys/ < media-keys.dconf

