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

![Screenshot 2026-03-11 105026.png](attachment:85042cdf-853a-418c-8b9c-b584610f1a72:Screenshot_2026-03-11_105026.png)

Open Oracle VirtualBox and create a new virtual machine for Windows Server 202. I named it 'Server 2022', stored it at C:\Users\hamed\VirtualBox VMs, set the OS to Microsoft Windows 64-bit, and configured virtual hardware and hard disk settings.

![Screenshot 2026-03-11 105300.png](attachment:41876012-c370-405d-92ec-cd0b2c480140:Screenshot_2026-03-11_105300.png)

I mounted the ISO file and started the virtual machine. This allowed the system to boot into the Windows installation setup.

![Screenshot 2026-03-11 105435.png](attachment:47c05edb-5b27-41df-a34f-55b315ae3339:Screenshot_2026-03-11_105435.png)

After completing the installation, I logged in using Ctrl+Alt+Delete. Server Manager launched
automatically on login

![Screenshot 2026-03-11 110859.png](attachment:4084885b-e565-4301-a67a-baba183d6e63:Screenshot_2026-03-11_110859.png)

I’m inside the server now. Server Manager popped up automatically. 

![Screenshot 2026-03-11 111012.png](attachment:fec964e3-7275-491c-93cb-b09953ad479d:Screenshot_2026-03-11_111012.png)

With Server Manager open, I navigated to Settings > System > About and clicked 'Rename this PC'.
The default random name WIN-HSMK57FVOL8 was replaced with HOUTECH01. After restarting, the
system confirmed the name change would take effect.

![Screenshot 2026-03-11 114851.png](attachment:cbda2acf-0bfd-483e-b124-0bde06700fc0:Screenshot_2026-03-11_114851.png)

![Screenshot 2026-03-11 125056.png](attachment:977928a6-fdb2-4dfb-b716-6c3b5b57f6b5:Screenshot_2026-03-11_125056.png)

I started the Windows 11 installation process.

This began the setup of the operating system from scratch.

![Screenshot 2026-03-13 095227.png](attachment:655dfe28-797e-4ead-9f69-d58fc545d7be:Screenshot_2026-03-13_095227.png)

Choosing Windows 11 Pro over Home is a technically critical decision. Windows 11 Home does not support domain joining. Only Pro, Education, and Enterprise editions support Active Directory domain membership.

![Screenshot 2026-03-13 095340.png](attachment:5d3e1aef-3754-4851-b376-6df9a8d5eb80:Screenshot_2026-03-13_095340.png)

During the Windows 11 Out-of-Box Experience (OOBE), I was prompted to give the PC a name before the desktop loaded

![Screenshot 2026-03-13 100626.png](attachment:8e582b08-606f-47c3-b5fd-59140309bde2:Screenshot_2026-03-13_100626.png)

I entered a local username and clicked Next I set a password, clicked Next, and completed the security questions

![Screenshot 2026-03-13 104616.png](attachment:1f3f8c19-612b-4cf9-80b4-4a684e0a18db:Screenshot_2026-03-13_104616.png)

I verified the installation and checked system details. This confirmed everything is working properly after setup.

![Screenshot 2026-03-13 105603.png](attachment:c6798760-372f-446e-884a-bc8edfb08a07:Screenshot_2026-03-13_105603.png)
