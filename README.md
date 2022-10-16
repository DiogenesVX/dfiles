# dfiles
A simple file manager for Linux/Sway/Wayland.
DFiles is a simple file manager that supports the basic file operations, it uses yad for the interface.
I used to use Thunar and Nautilus file managers on Sway/Wayland (with disabled Xwayland) but they pull in a few dependencies especially Nautilus is annoying because it depends on those tracker-miners which use quite a bit of resources and moreover are completely useless for me personally, so I decided to create a simple file manager to do basic file operations whenever I'm too lazy to open a terminal :). I created it for myself to use with Sway on Debian. If someone finds it useful for his/her situation, I'd be happy :).

# What you can do with dfiles
   1. Browse your files and directories.
   2. Do a quick search, quickly navigate to the path you need.
   3. Create a new file/directory, rename/copy/cut/delete selected files/directories.
   4. Open the terminal in the current location (by default the foot terminal is used so either install foot or modify the code).
   5. Display file/directory information.
   6. Manage USB and Android devices (mount/unmount).
   7. Manage the mimetypes (add/edit/reset).
   8. Supports icon themes and icon sizes (provided by the theme, some non-standard themes might not work).

# Screenshots
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/dfiles.png)
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/dfiles-options.png)
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/breeze-dark-22.png)
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/breeze-dark-64.png)
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/adwaita.png)
![Alt text](https://github.com/DiogenesVX/dfiles/blob/main/dfiles-mimetype-editor.png)

# Usage
  1. For the correct work, place the dfiles script into /usr/local/bin/
  2. Just start it by typing in terminal: dfiles
  3. Also you can add the following to your sway config (to open it by pressing super+t):
  
         bindsym $mod+t exec --no-startup-id dfiles
  
 Make sure you have the following packages installed:

        sed
        yad
        bash
        grep
        gawk
        procps
        coreutils
        findutils
        util-linux
        adwaita-icon-theme
        fonts-noto-color-emoji
        
 Optional packages (if you need support for notifications, mounting devices etc.)

        dunst
        fuse3
        jmtpfs
        udisks2
        libnotify-bin
