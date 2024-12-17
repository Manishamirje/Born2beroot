# Born2beroot

Refer for Born2beroot - https://haglobah.github.io/Mastering-42/holy_graph/born2beroot.html 


https://tldp.org/HOWTO/Unix-and-Internet-Fundamentals-HOWTO/anatomy.html chapter 2 to 10

https://github.com/pasqualerossi/Born2BeRoot-Guide/blob/main/README.md 

https://github.com/HEADLIGHTER/Born2BeRoot-42/blob/main/walkthrough37.txt - very helpful with nano feels easy to edit files

https://github.com/gemartin99/Born2beroot-Tutorial/blob/main/README_EN.md

https://github.com/PublioElio/School-42-Born2beroot - has everything for eval knowledge


  You should know the following:
SSh - Secured Socket Shell

Crontab -

GRUB - Grand Unified Bootloader

LVM - Logical Volume Manager

UFW - Uncomplicated Firewall

vdi - virtual(Box) disk image

iso - Identical Storage Image

AppArmor - Low - level Package manager

SeLinux - Security-Enhanced Linux

Vim and Nano - text Editors


To check files and configuration files (for Eval):
  lsblk - Check - partitions

  Sudo aa-status - AppArmor status
  
  getent group sudo - Sudo group users
  
  Getent group user42 - User42 group users
  
  Sudo service ssh status - Ssh status
  
  Sudo ufw status - Ufw status
  
  Ssh username@ipadress -p 4242 - Connect to VM from your host (physical) machine via SSH
  
  Nano /etc/sudoers.d/<filename> - Sudo configure file. You can $ ls /etc/sudoers.d first
  
  nano /etc/login.defs - password expire policy
  
  nano /etc/pam.d/common-password - password policy
  
  sudo crontab -l - cron schedule

UFW - UFW, or Uncomplicated Firewall, is an interface to iptables that is geared towards simplifying the process of configuring a firewall.
Uncomplicated Firewall (UFW) is a program for managing a netfilter firewall designed to be easy to use. It uses a command-line interface consisting of a small number of simple commands, and uses iptables for configuration. UFW is available by default in all Ubuntu installations since 8.04 LTS. UFW has been available by default in all Debian installations since 10.

.vdi - A virtual disk image (VDI) is defined as the image of a virtual hard disk or the logical disk associated with a virtual machine. A virtual hard disk (VHD) is a disk image file format used to virtualize the contents of a computer's hard drive.

.iso - What is an ISO file extension? An ISO file is, simply put, a digital file format replicating a physical CD, DVD, or BD. The ISO file extension does not just store files and folders; they house all the vital file system information about the disc's structure.
The term “ISO file” or “ISO image” goes back to the standardized format ISO 9660 or 13346 for CD-ROM media and stands for the identical storage image of optical media. An ISO file thus contains all the same data you would transfer when copying data to CD, DVD, or Blu-ray.

Nano is a modeless editor and works in a single mode. Vim is a mode-based editor. Nano is a WYSIWYG (What You See Is What You Get) command-line editor. Vim is not a WYSIWYG text editor.

**Vim** is highly customizable and extensible, making it an attractive tool for users who demand a large amount of control and flexibility over their text editing environment. 

**Is Vim a programming language?**
To add new features like keyboard shortcuts, one can use Vim script, Vim's built-in programming language. Many Vim plugins and extensions are also available online for free. There is an Internet turf war between programmers that prefer Vim and programmers that prefer Emacs, another common text editor.

**Nano** is a simple command-line text editor commonly found in Unix-based operating systems. It allows users to quickly edit text files directly from the command line. The editor's intuitive interface and keyboard shortcuts make it convenient for editing configuration files, scripts, and other text-based documents.


Difference between SELinux and APPArmor?

“These security systems provide tools to isolate applications from each other and in turn isolate an attacker from the rest of the system when an application is compromised.

SELinux rule sets are incredibly complex but with this complexity you have more control over how processes are isolated. Generating these policies can be automated. A strike against this security system is that its very difficult to independently verify.

**Security-Enhanced Linux (SELinux)** is a Linux kernel security module that provides a mechanism for supporting access control security policies, including mandatory access controls (MAC). SELinux defines access controls for the applications, processes, and files on a system.

**AppArmor** (and SMACK) is very straight forward. The profiles can be hand written by humans, or generated using aa-logprof. AppArmor uses path based control, making the system more transparent so it can be independently verified.” (source)
