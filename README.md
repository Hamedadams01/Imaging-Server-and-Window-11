# Installing Server & Windows 11

**Overview**

---

In this lab, I prepared a virtualized enterprise environment by installing both Windows Server 2022 and Windows 11 Pro inside Oracle VirtualBox. The goal was to simulate a real-world IT setup that mirrors what is found in corporate environments — a domain controller running Server 2022 and a domain-joined client machine running Windows 11 Pro. This lab forms the foundation for all subsequent labs including Active Directory setup, Group Policy configuration, and helpdesk ticketing workflows.

**Objectives**

---

- Download and select the correct ISO files for Windows Server 2022 and Windows 11 Pro.
• Create and configure two virtual machines in Oracle VirtualBox.
• Successfully install Windows Server 2022 and boot into Server Manager.
• Rename the server to HOUTECH01 following organizational naming standards.
• Install Windows 11 Pro (not Home) to support domain joining in future labs.
• Complete the Windows 11 Out-of-Box Experience (OOBE) and verify system specifications.

**Documentation**

---

On this step, I prepared the environment by downloading and selecting the correct ISO files for both Windows Server and Windows 11. This was important because choosing the correct system images ensures compatibility and allows me to properly simulate a real-world enterprise setup.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_105026.webp)

Open Oracle VirtualBox and create a new virtual machine for Windows Server 202. I named it 'Server 2022', stored it at C:\Users\hamed\VirtualBox VMs, set the OS to Microsoft Windows 64-bit, and configured virtual hardware and hard disk settings.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_105300.webp)

I mounted the ISO file and started the virtual machine. This allowed the system to boot into the Windows installation setup.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_105435.webp)

After completing the installation, I logged in using Ctrl+Alt+Delete. Server Manager launched
automatically on login

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_110859.webp)

I’m inside the server now. Server Manager popped up automatically. 

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_111012.webp)

With Server Manager open, I navigated to Settings > System > About and clicked 'Rename this PC'.
The default random name WIN-HSMK57FVOL8 was replaced with HOUTECH01. After restarting, the
system confirmed the name change would take effect.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_114851.webp)
![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-11_125056.webp)

I started the Windows 11 installation process.

This began the setup of the operating system from scratch.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-13_095227.webp)
Choosing Windows 11 Pro over Home is a technically critical decision. Windows 11 Home does not support domain joining. Only Pro, Education, and Enterprise editions support Active Directory domain membership.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-13_095340.webp)
During the Windows 11 Out-of-Box Experience (OOBE), I was prompted to give the PC a name before the desktop loaded

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-13_100626.webp)

I entered a local username and clicked Next I set a password, clicked Next, and completed the security questions

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-13_104616.webp)
I verified the installation and checked system details. This confirmed everything is working properly after setup.

![image alt](https://github.com/Hamedadams01/Imaging-Server-and-Window-11/blob/2d44a88e044e60dffe09fb6e8f92108ee6a93266/Screenshot_2026-03-13_105603.webp)
