# My own Gnome keybindings for a tiled desktop
I recently started tiling windows on my desktop with the Gnome
Tiling Shell extension. 

The Gnome + Tiling Shell approach works great and provides me with a Gnome desktop environment that resembles Hyprland for those hyprfocused moments yet keeps the sweet usability of Gnome when you're in a rush.

Hyprland is fantastic! But it's a pain when you're in a rush to deliver. When the pressure's on - I work as a CTO, the pressure's on basically... daily! - there's nothing like a desktop GUI metaphore that keeps you from mental madness.

Yet, tiling is great when you need to relax, take a step back, analyze the the hole
picture. Hence I managed to dive into a solution that provides me with the best of
both world, aka the fixibility of the Gnome desktop and the rigorous tile-centrit
windows arrangement of Hyprland.

This is a very much a personal repo, I'm making it public just for the sake of
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

Ok, you're done!

## Bonus: GTK styling with CSS
My own GTK styling with CSS, no theme extensions of tweaks required! Copy files gtk-3.css and gtk-4.css from this repo directory to ~/.config/gtk-3/ and ~/.config/gtk-4/.

cp gtk-3.css ~/.config/gtk-3/gtk.css

cp gtk-4.css ~/.config/gtk-4/gtk.css

