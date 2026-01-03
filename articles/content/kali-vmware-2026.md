---
title: Setting up Kali Linux in VMware (2026)
date: 2026-02-14
tags: kali, vmware, security
---

## Overview

This guide walks through setting up a **Kali Linux virtual machine** on **Windows 11** using VMware Workstation Pro.  

It assumes basic familiarity with virtualization, but no prior Kali experience is required.

### Assumptions

- Windows 11 host operating system
- Hardware virtualization enabled in BIOS (VT-x / AMD-V)
- At least 16GB RAM recommended (8GB minimum)

---

## Step 1: Download VMware Workstation

Download VMware Workstation Pro from the official website:

[VMware Workstation Pro](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

![VMware Download Page](/images/vmware_download.png "VMware Download")

Click **Download Now** under VMware Workstation Pro for PC. You will be redirected to the Broadcom Support portal.  
Create an account if needed, then navigate to **My Downloads → Free Software Downloads**.

![Broadcom Free Download Link](/images/broadcom_free_download.png "Broadcom Free Download Link")


Select the version you want and download the `.exe` installer. Run it and follow the prompts to install VMware Workstation.

---

## Step 2: Download the Kali Linux Virtual Machine

Visit the official Kali VM page:

[Kali Linux Virtual Machines](https://www.kali.org/get-kali/#kali-virtual-machines)

Download the VMware version. The **torrent option** is faster and more reliable, but the direct website download also works.  

Once downloaded, extract the archive using a tool like **7-Zip**. For convenience, place the extracted files in their own folder.

---

## Step 3: Set Up the Virtual Machine

1. Open VMware Workstation.
2. Go to **File → Open** and select the `.vmx` file from the extracted Kali VM folder.
3. Before powering on the VM, click **Upgrade this virtual machine** and choose the VMware version you installed.  
   > Skipping this step may result in the mouse cursor not working inside the VM.
4. Power on the virtual machine.

### Default Login Credentials

- **Username:** `kali`
- **Password:** `kali`

---

## Step 4: Common Issues

**No mouse cursor inside VM**  
- This usually happens if the VM upgrade step is skipped.  
- Fix: VM → Upgrade Virtual Machine → Match installed VMware version.

**VM won’t start / snapshot errors**  
- Make sure hardware virtualization is enabled in BIOS.  
- Ensure your host system has enough RAM.

---

## Conclusion

You now have a fully functional Kali Linux virtual machine ready for security testing and learning.  

From here, you can start exploring Kali’s tools, practice penetration testing in a safe environment, or use it for your lab projects.
