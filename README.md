# Flashing firmware from start (Jetson TK1):
- [Read PDF provided by Nvidia](Jeston_TK1_User_Guide.pdf)
- Note - Password for ubuntu account is ubuntu.

# Upgrade from Ubuntu 14.04 to 16.04
- Run the following command:
```sudo do-release-upgrade```
- Note - Say yes to every prompt.

# Install drivers for Intel 7260 AC board
- [Refer to this website for the information](https://elinux.org/Jetson/Network_Adapters)
- [Please use this driver file and copy it to /lib/firmware/](iwlwifi-7260-14.ucode)
- Install Linux-firmware, load kernel module, and reboot using these command:
```
sudo apt install linux-firmware
sudo modprobe -r iwlwifi
sudo modprobe iwlwifi
sudo reboot
```
