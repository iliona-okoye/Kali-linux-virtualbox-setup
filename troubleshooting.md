# Troubleshooting

## VM won't boot / black screen
- Make sure virtualization (Intel VT-x / AMD-V) is enabled in your BIOS/UEFI settings
- Check that the Kali ISO is properly attached under VM Settings → Storage

## "VT-x is not available" error
- Enable virtualization in your BIOS/UEFI
- On Windows, disable Hyper-V and Windows Sandbox if enabled (they can conflict with VirtualBox), via **Control Panel → Programs → Turn Windows features on or off**

## Installation is very slow
- Increase allocated RAM and CPU cores in VM Settings
- Make sure you're using a Dynamically Allocated VDI, not Fixed size, if disk space is limited

## No internet access inside the VM
- Check Network settings — NAT should work out of the box for most cases
- Try switching to Bridged Adapter if NAT isn't working

## Screen resolution is stuck / too small
- Install VirtualBox Guest Additions (see Step 5: Post-Install Setup)
- Restart the VM after installing Guest Additions

## Guest Additions install fails
- Run `sudo apt update` first, then retry `sudo apt install -y virtualbox-guest-utils`
- Make sure the Guest Additions CD image is mounted via Devices menu in the VirtualBox window
