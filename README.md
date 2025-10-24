# My own Gnome keybindings (for a tiled desktop)
I recently started tiling windows on my desktop with the Gnome
Tiling Shell extension. This approach works great to have a Gnome
desktop environment that resembles Hyprland for those hyprfocused
moments yet keeps the sweet usability of Gnome when you're in a rush.

It's very much a personal repo, I'm making it public just for the sake of
someone possibly benefiting from it.

### Preconditions
Install Gnome Extensions Manager
Install extention Tiling Shell (beautiful work!)

### Export all Gnome keybindings from one PC
dconf dump /org/gnome/desktop/wm/keybindings/ > gnome-keybindings.dconf
dconf dump /org/gnome/settings-daemon/plugins/media-keys/ > media-keys.dconf

### Export all Tiling Shell keybindings from one PC
Use the extension floating window, export button.

### Import all keybindings on the other PC
dconf load /org/gnome/desktop/wm/keybindings/ < gnome-keybindings.dconf
dconf load /org/gnome/settings-daemon/plugins/media-keys/ < media-keys.dconf

### Import Tiling Shell keybindings on the other PC
Use the extension floating window, import button.

Ok, you're done.
