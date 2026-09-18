# Step 5: Post-Install Setup

## Install VirtualBox Guest Additions
Guest Additions improve performance and enable features like shared clipboard, drag-and-drop, and better screen resolution.

1. Start your Kali VM and log in
2. In the VirtualBox window menu, go to **Devices → Insert Guest Additions CD image**
3. Open a terminal in Kali and run: sudo apt update
sudo apt install -y virtualbox-guest-utils
4. Reboot the VM:sudo reboot
## Update the system
Keep Kali current with the latest packages and security patches: sudo apt update && sudo apt full-upgrade -y
## Create a snapshot
Snapshots let you save your VM's current state and roll back if something breaks later (very useful before trying new tools or configurations).

1. In VirtualBox Manager, select your Kali VM
2. Go to **Snapshots** tab
3. Click **Take**
4. Name it something like `Clean Install` or `Post-Setup`

## Adjust display resolution (if needed)
With Guest Additions installed, you can usually resize the VM window and the resolution will scale automatically. If not, check: xrandr to see available resolutions.

## You're done
Your Kali Linux VM is now installed, updated, and ready for use. Future snapshots let you experiment safely and roll back whenever needed.
