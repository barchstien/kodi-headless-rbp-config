On Raspberry Pi 3
# Install & Config
  1. Install ArchArm [Official 
Docs](https://archlinuxarm.org/platforms/armv8/broadcom/raspberry-pi-3)
  2. Update Arch and install kodi-rsbp  
    `pacman -Syu`  
    `pacman -S kodi-rsbp`
  3. Copy/modify guisettings.xml  
    `cp userdata/guisettings.xml /var/lib/kodi/.kodi/userdata/`  
    This file contains config for using HifiBerry DAC + and to rnu the Web Interface
  4. Copy/modify sources.xml
    This file contains examples to setup media sources

# Run
As root, run `systemctl start|stop kodi`  
This runs kodi as user kodi, and kodi home directory is **/var/lib/kodi**

Enable at boot with  
  `systemctl enable kodi`
