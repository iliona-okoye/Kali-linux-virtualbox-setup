# Step 4: Installing Kali Linux

## Boot the VM
1. In VirtualBox Manager, select your Kali VM
2. Click **Start**
3. The VM will boot from the attached ISO into the Kali installer menu

## Choose install mode
- Select **Graphical Install** (easier for beginners) using arrow keys, then press Enter

## Installation walkthrough
1. **Select a language** → choose your preferred language
2. **Select your location** → choose your country/region
3. **Configure the keyboard** → choose your keyboard layout
4. **Configure the network:**
   - Enter a **hostname** (e.g. `kali`)
   - Enter a **domain name** (can leave blank)
5. **Set up users and passwords:**
   - Set a **root password** (or configure a regular user, depending on Kali version)
6. **Configure the clock** → select your timezone

## Partition the disk
1. Choose **Guided – use entire disk** (simplest option for a VM)
2. Select the virtual disk you created in Step 3
3. Choose **All files in one partition** (recommended for beginners)
4. Confirm and write changes to disk when prompted

## Software selection
- Keep the default Kali metapackages selected (or customize if you know which tools you want)
- Wait for installation to complete — this can take 15–30 minutes depending on your host machine

## Install GRUB bootloader
1. Choose **Yes** to install GRUB
2. Select the virtual disk (not a separate device) as the install location

## Finish installation
1. Once complete, select **Continue** to reboot
2. Remove the ISO from the virtual drive (VirtualBox usually does this automatically) so it boots into your new Kali install instead of the installer again

## Verify
You should now boot into the Kali Linux login screen.

## Next step
→ [Post-Install Setup](05-post-install-setup.md)
