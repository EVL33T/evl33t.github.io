---
title: Install Kali in VirtualBox
layout: post
date: 2018-03-09 00:00:00 +0000
published: true
categories: []
---
Kali is the most popular pen testing linux distros, and installing it on your computer is hard, so let's do it in VirtualBox.

## 1. Download VirtualBox

Download the VirtualBox for your OS from here: [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads "https://www.virtualbox.org/wiki/Downloads")

Install it as you would any other software.

If you're running linux, try looking for it in your package repos.

## 2. Download a Kali ISO

Download a Kali ISO from here: [https://www.kali.org/downloads/](https://www.kali.org/downloads/ "https://www.kali.org/downloads/")

The "Full-64bit" one should be fine, but feel free to choose another one if you have limited space or a different DE preference.

Note: Do NOT download the VirtualBox image, that isn't frequently updated and is unreliable.

## 3. Create a new VM

Open VirtualBox, and click new. Choose these settings:

![](/media/VM-create-1024x591.png)

You can change the RAM and name as you wish, but keep the RAM at least 2 GB, but less than half of your total system RAM. Click Create.

Again, choose these settings:

![](/media/Disk-create-1024x578.png)

You can change the name and file size, of course, but make sure to give it at least 20GB.

Click on your newly created VM, then go to Settings -> Network -> Adapter1 and change the "Attached to" to Bridged Adapter. (This means that Kali will use your network card directly, and will make it easier to hack wifi/other things)

## 4. Start your VM

Click start. Click the folder icon, and browse to the downloaded Kali ISO.

Down-arrow to "Graphical Install" and press enter.

## 5. Install the system

Just follow the instructions - these should be straightforward enough.

Some important settings:

* When choosing how to partition the disk, choose "Guided-Use whole disk"
* Keep all folders in same partition
* Install grub to /dev/sda

Comment if you have any issues with this.