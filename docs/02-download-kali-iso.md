# Step 2: Downloading Kali Linux

## Official download page
Go to the official Kali Linux downloads page: https://www.kali.org/get-kali/

## Choose the right image
For VirtualBox, you have two options:

### Option A: Pre-built VirtualBox image (easier)
1. Under **Virtual Machines**, select **VirtualBox**
2. Download the 64-bit image
3. This comes as a compressed file — extract it after downloading
4. Skip most of Step 3 (VM creation) since the VM is pre-configured — just open it directly in VirtualBox via **File → Import Appliance**

### Option B: ISO installer image (more control, recommended for learning)
1. Under **Installer Images**, select the 64-bit **Installer** ISO
2. This is a standard `.iso` file you'll attach to a VM you build yourself (covered in Step 3)

This guide follows **Option B**, since building the VM yourself teaches you more about the process.

## Verify the download (optional but good practice)
Kali provides SHA256 checksums on the download page. After downloading, you can verify the file wasn't corrupted or tampered with by comparing checksums — most OS have a built-in way to do this (e.g. `sha256sum` on Linux/Mac, `Get-FileHash` in PowerShell on Windows).

## Next step
→ [Creating the VM](03-vm-configuration.md)
