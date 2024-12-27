# VirtualBoxInstructions
This repository contains instructions on how to set up Virtualbox with Ubuntu image.


## Getting Started
1. Install Virtualbox application: https://www.virtualbox.org/wiki/Downloads
2. Install Ubuntu image.
   - https://releases.ubuntu.com/jammy/
3. Once Virtualbox is installed, create a new VM
    - Note:
      - Name of virtual machine cannot have space
      - Select ISO image, this should fill in default for type and version
      - Enable skip unattended installation to not install Guest Additions (Guest Addistion ISO needs to be installed)
4. Once specified the specs of virtual box, enable bidirectional copy
  - Go to Settings -> Advanced -> Shared Clipboard 
5. Start the Ubuntu VM
6. Go for minimal installation (can go non-minimal)
7. Add Wifi installation
8. If you have not installed Guest Addition ISO, then can install through terminal.
  - `sudo apt install build-essential dkms linux-headers-$(uname -r)`
9. If went for minimal installation, install basic packages
  - `sudo apt-get install build-essential gcc make perl dkms`
10. Once installed, go to Devices -> Insert Guest Addition ISO
11. Go to the mounted Vbox disc (e.g. `cd /media/<user>/VBox_GAs_7.1.4/`)
    - Get the VBox Linux Addition
      - `sudo ./VboxLinuxAdditions.run`
12. Reboot
13. Enable bidirectional copy

   
