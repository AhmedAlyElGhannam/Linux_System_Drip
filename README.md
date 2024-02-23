# Linux Drip Setup Speedrun
Yo! Wussup muh daug! Yo Linux system be bussin with these nibbas down below. Check dem out!


## Gnome Extensions
1. Install Chrome from the url:
   ```
   https://www.google.com/chrome/next-steps.html?statcb=1&installdataindex=empty&defaultbrowser=0&brand=JJTC&gad_source=1&gclid=Cj0KCQiAoeGuBhCBARIsAGfKY7xJBmvs0lvPbf3VUiwhf-RCEjnlJE3HGZkCRTpVtfpDRpTWIy6wPX0aAt5aEALw_wcB&gclsrc=aw.ds
   ```
   
1. Enable Gnome Extention Plugin in Chrome + Install essential shit:
   ```
   https://chromewebstore.google.com/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep
   ```
   ```
   sudo apt install chrome-gnome-shell
   ```
   
1. Go to ![Gnome Shell Extensions website](https://extensions.gnome.org/) and set up the following stuff:
   1. Dash to Dock.
   1. Blur My Shell.

1. Do not forgot to install `Gnome Extension Manager` from Ubuntu Store.


## Papirus Icon Pack
1. Run this:
   ```
   sudo add-apt-repository ppa:papirus/papirus
   ```

1. Install that:
   ```
   sudo apt update && sudo apt install papirus-icon-theme
   ```

1. In order to change icon pack, install `Gnome Tweaks` from Ubuntu Store.


## Neofetch Terminal Drip
This will be a summary of how I made the drippiest drip for my terminal.

1. Install neofetch
   
   ```
   sudo apt install neofetch
   ```
   
2. Enter the following command to open neofetch settings
   
   ```
   sudo gedit /usr/bin/neofetch
   ```
   
3. Remove any of the existing OS's logos and put L-Drago SIZE=60 in its place. I removed Red Star just because it fits L-Drago's aesthetics. Do not forget to save before exiting.

4. Open neofetch's config file. You have to open neofetch AT LEAST ONCE for in order for this file to be generated.
   
   ```
   sudo gedit ~/.config/neofetch/config.conf
   ```
   
5. Only show the following:
   
   ```
    info title
    info underline
    info "OS" distro
    info "Host" model
    info "Kernel" kernel
    info "Uptime" uptime
    info "Resolution" resolution
    info "CPU" cpu
    info "GPU" gpu
    info "Memory" memory
    info "Disk" disk
   ```
   
6. Search for `ascii_distro` and change it to the distro you placed L-Drago as its logo. Save before exiting.

   ```
   ascii_distro="Red Star"
   ```
   
7. To run neofetch every time the terminal starts, add it to `.bashrc`.
    
   ```
   vim ~/.bashrc
   /* write neofetch at the end of the file + save before exiting */
   neofetch
   ```
   
8. Source bashrc after exiting to load changes.
    
   ```
   source ~/.bashrc
   ```
   
9. Profit!
    
    ![](drip.png)
