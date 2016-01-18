---
layout: post
title:  "The Great Upgrade of 2015"
date:   2016-01-06 23:00:55
categories: environment
banner_image: xps-13.png
comments: true
---
Recently, I started the long switch to linux after switching between Windows and Mac OS X for years. I chose Ubuntu 15.10 Unity, and decided on the Dell XPS 15 with the UltraHD display and Skylake CPU. It's roughly the same weight as my customer's 15" MacBook Pro... but with easily twice the power. However, it's been a *lot harder than it should have been*.

### The Challenges
1. The BIOS ships with the microphone disabled, and due to a bug in A05 will refuse to enable it.
1. The HDMI port will lockup Ubuntu, but might work in Windows 10.
1. The BIOS ships with the drive controller set to RAID even though the device only has one drive.
1. The UEFI and BIOS basically will fight any attempt to install an OS (fastboot, secure boot, etc, etc, etc.)
1. The thunderbolt port requires a TypeC adapter (~$16).
1. The BIOS ships with the Thunderbolt 3 port disabled, and due to a bug in A05 will refuse to enable it.
1. Since Dell does not directly support Ubuntu for the XPS 15,  there is **no way to get video externally yet**. So my happy P2415Q (UHD) can't extend my desktop yet.
1. Native apps are not all the way there yet. Especially on HiDPI.
1. Wine is a joke, and before you say it - *I chose Ubuntu to use containers - not a full VM*.

After days of confusion, missteps, hand wringing, calls for assassinations and cursing I was able to boot from a USB stick, install Ubuntu and setup a dual boot with Windows 10.

### OS Installation
I chose Ubuntu 15.10 in my case. Be prepared to want to commit sepuku half way through... because without an advanced sorcering degree in *linux-think* you will want it all to end. I especially appreciated all the headaches with the grub2 loader and the confusing array of scaling options for HiDPI that Java just happens to totally ignore.

### Post OS Installation
Now comes the fun part. The post install configuration. I set out with a desire to setup a bunch of software I need on a day to day basis, plus Steam and a finance app I use. I found out that the Software Center is way out of date and most people use apt-get anyway. Meanwhile, the Synaptic Package Manager seems to be the only way to force an older version. 
>**Sidenote**: Dude. Maybe npm, inc. should do a Linux package manager!

##### Ubuntu apps:
* **WebStorm 11** (which has gone up in price from $29/yr to $77/yr, while simultaneously getting slower)
* **Visual Studio Code** (which will ultimately replace WebStorm)
* **HipChat** (which is honestly garbage on Linux)
* **Slack**
* **Skype**

##### Windows apps via Wine
I initially thought, no worries I can install what I miss (Outlook, OneNote, Evernote, SourceTree and the finance app) under Wine. After days of messing around with Wine version security issues randomly preventing apps from running, then failing with *winetricks*, then switching to **PlayOnLinux** to natively support multiple versions of wine... I eventually gave up and switched to Web Apps.

* For Outlook, I decided to try **Evolution** with my customer address for now.
* For SourceTree, I gave up and decided to try **GitKraken**. Install and review, pending.

> **Sidenote**: But forget Wine, it's old and busted.
**Web Apps have finally arrived**. Here's [how to do it](#).