+++
title = 'Trial By Boot'
date = 2026-02-05T15:57:54Z
subtitle = 'My attempts at recompiling the Linux Kernel on Ubuntu.'
draft = false
+++
## My attempts at recompiling the Linux Kernel on Ubuntu.

As a daily Linux user, I consider it to a right of passage to recompile the Linux Kernel at least once.  But what started as a fun little weekend project turned into weeks of frustration and a laptop that couldn't access its own file system.

It began so well, I was following a guide, determining which 'modules' I could dispense with, for a leaner and hopefully more responsive system and seeing other cool modules I could add to experiment with.  However, I quickly noticed a distinct lack of a Open ZFS module, which I understand to be a DKMS module usually. This was unfortunate as, at the time, I was using Ubuntu's Experimental ZFS support as my filesystem.  This turned out to be the origin of the chaos I later experienced. 

At first, everything seemed good, I followed the instructions to the letter, I manually installed ZFS from the package-manager and then I rebooted.

*This was when the grief started.*

At first, GRUB loaded, I selected my new Kernel and waited for it to boot.

Then after loading the Initial RAM File System, 'Initramfs', it hang, then Kernel Panic'd. 

Reading the console, it showed that my new kernel lacked the ZFS Driver, the one usually provided by the ZFS DKMS Package.  Meaning my file system, beyond the boot partition, was unreadable by my own kernel.

Now this had happened to me before, when, in Sixth Form, I attempted to update the Kernel of my PC through the Package Manager (APT/DEB/DPKG) but this failed more spectactuarly and for essentially the same reason.  I had neglected to update the ZFS DKMS module, but instead of the hang then panic, the Kernel Panic'd immediately and I ended up having to entirely wipe the boot drive and start again.  This did lead down the path of learning NixOS but that is covered elsewhere on this site.

Luckily, on this occasion, I was somewhat able to salvage the Ubuntu Installation, although not enough to prevent myself from just Distro-Hopping to Rocky 10 (EPEL 10 based Linux).  The salvage was made possible as I hadn't deleted the old GRUB entries for the Stock Kernel and as such I was able to boot back into the install, thus permitting the backup of some important files on the drive.

A consequence of this is that I will not be recompiling Linux Kernels again for a little while.