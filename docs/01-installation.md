# 📦 Windows Server 2022 Installation Guide

This guide walks you through downloading, installing, and configuring Windows Server 2022 in your SOC HomeLab using VirtualBox. This documentation is part of my ongoing series on building a realistic, hands-on SOC lab environment.

---

## 🔗 Downloading Windows Server 2022

1. Go to the official evaluation center:  
   👉 [https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022)

2. Click on **"Download the ISO"**.

3. Fill out the required information (Name, Email, Company, etc.).

4. Choose the ISO for your system architecture and download it.

---

## 🧰 VirtualBox Settings

Once the ISO is downloaded, set up your virtual machine in VirtualBox:

1. Open VirtualBox and click **"New"**.

2. Name your VM (e.g., `WindowsServer2022`) and choose the appropriate version (`Windows 2022 (64-bit)`).

3. Allocate system resources:
   - RAM: Minimum **4 GB** (8 GB recommended)
   - CPU: At least **2 cores**

4. On **Hard disk**, choose:
   - **Create a virtual hard disk now**
   - **VDI (VirtualBox Disk Image)**
   - **Dynamically allocated**
   - Disk size: At least **40 GB**

5. Go to **Settings > Storage**:
   - Under "Controller: IDE", click the empty CD icon.
   - Attach the downloaded **Windows Server 2022 ISO**.

6. Adjust network settings:
   - Use **Bridged Adapter** or **Internal Network** depending on your lab configuration.

---

## 🖼️ Screenshots

You can reference the screenshots below for proper setup:

- ![vm1](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm1.png)
- ![vm2](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm2.png)
- ![vm3](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm3.png)
- ![vm4](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm4.png)
- ![vm5](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm5.png)
- ![vm6](https://ld-images-2.s3.us-east-2.amazonaws.com/Building+a+SOC+Lab+at+Home/02-ActiveDirectory/Images/Images/vm6.png)

---

Once the installation completes, you’ll be prompted to:
- Set an Administrator password
- Customize settings
- Begin initial configuration

📌 Now you're ready to proceed to the next steps:
1. Setting a Static IP  
2. Configuring Active Directory (AD)  
3. Promoting the server to a Domain Controller (DC)

These will be covered in the next parts of this documentation series.

---

**Author:** *@ladysheraz — SOC HomeLab Project*  
**Tags:** `#SOC`, `#WindowsServer2022`, `#BlueTeam`, `#Homelab`, `#ActiveDirectory`, `#Infosec`


