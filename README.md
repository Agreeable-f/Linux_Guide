# Step by step guide to your first time in Linux!

### This is an in-depth guide you through your first time using linux from being a complete beginner with computers.

### The method in this guide doesn't require you to install linux to try it out, however there will be instructions on how to do that as well.

### Contents
1. [Prep. Shopping list, terms, and information](#shopping_list)
    1. [Some important terms](#terms)
2. [Step 1. Getting Linux on your USB](#step1)
    1. [Option 1. Balena Etcher](#o1balena)
        1. [Downloading Balena](#dlbalena)
        2. [Using Etcher](#useetcher)
    2. [Option 2. Rufus](#o2rufus)
       1. [Downloading Rufus](#dlrufus)
        2. [Using Rufus](#userufus)
    3. [Option 3. Ventoy](#o3ventoy)
        1. [Downloading Ventoy](#dlventoy)
        2. [Setting up Ventoy](#suventoy)
        3. [Using Ventoy](#useventoy)
        4. [Putting your ISO on your USB](#isotoventoy)
3. [Step 2. Booting into Linux](#step2)
    1. [The BIOS](#bios)
        1. [Getting to your BIOS](#tobios)
        2. [Navigating your BIOS](#navbios)
    2. [Navigating Ventoy](#navventoy)
    3. [The Live Environment](#liveenv)
4. [Step 3. Learning Linux](#step3)

<div id='shopping_list'/>

# Prep. Shopping List, terms and information

### These are the things that you'll need to follow along with this guide. You probably already have these items laying around!

1. Usb drive with at least ~8GB or more. (you can probably get away with less, around 4GB, but you'll be pretty limited as to what you can do)

2. A pc running windows with a usb port. (while you *can* do this on an intel based mac but it's not covered in this guide)

3. A Linux ISO.  For this guide we'll be using Fedora Linux as it's a Stable Release packed with features.  
https://fedoraproject.org/workstation/download/

#### NOTE: You can use any distro you like. This guide just covers Fedora Linux but the steps until [Step 3.](#step3) are identical.

Scroll down until you find this section and click Download. We'll be using the Workstation version.

![Fedora Linux download button](Images/Fedora_Linux_download.png)

4. A tool to get the linux ISO on to the usb. (This will be covered in [Step 1.](#step1))

<div id='terms'/>

### Some important terms

<div id='Term_ISO'/>
- ISO: An ISO, also known as an *image*, is an archive, usually as a backup of optical media like CD's. In this case it's used to distribute a copy of linux. Not too different from physical install disks from back in the day.

<div id='Term_Distro'/>
- Distro: Distro, or distribution refers to the distribution of linux as there are many to chose from. Think of it like a supermarket. Target, Walmart, Kroger, Costco, would be the distributions or different choices under the umbrella term of "supermarket".

<div id='Term_Kernel'/>
- Kernel: The kernel is a computer program at the core of a computer that communicates between programs and things like your mouse and keyboard and tells everything what to do.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Kernel_%28operating_system%29

<div id='Term_DE'/>
- DE: DE is short for Desktop Environment. A Desktop Environment is a bundle of programs that allow you to interact with your computer. Think of your task bar and start menu. That's all part of the DE. In the case of this guide we'll be using one called Plasma by KDE. gnome is also a different DE.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Desktop_environment

<div id='Term_WM'/>
- WM: WM is short for Window Manager. A Window Manager is software that, as the name implies, manages your windows (the little boxes of programs that show up on your screen like google). The window manager mainly handles their position and how they move around, though that's a gross oversimplification.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Window_manager

<div id='Term_Package_Manager'/>
- Package manager: A package manager is as the name implies what manages all the packages on your system. The packages on your system is what makes up the software you have installed.

<div id='Term_Bootloader'/>
- BootLoader: A BootLoader is a program that boots up your Operating System. Which in our case is Linux.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Bootloader

<div id='Term_Linux'/>
- Linux: Linux refers to the Linux kernel itself, Though people often associate it with the full operating system.
For more context (and an inside joke with the linux community) see this copypasta https://stallman-copypasta.github.io/

<div id='step1'/>

# Step 1. Getting Linux on your USB

### For putting Linux on the USB we have a few options. Doing any one of which will remove everything on your USB drive so make sure you have everything backed up.

<div id='o1balena'/>

## Option 1. Balena Etcher (We'll be using this option for the rest of the guide.)

Balena Etcher etches or burns the image on to that USB. Similar to burning a CD back in the day. This means that you will only be able to boot to that single ISO or image that's burned to that USB drive. Though much more limited this method is alot simpler and will serve it's purpose for this guide.

#### NOTE: You can use your USB drive for other things after this. You'll just have to format your drive.

<div id='dlbalena'/>

### Downloading Balena Etcher

Doanload link: https://etcher.balena.io/#download-etcher

For Balena Etcher we'll use the portable version as it skips the need to install.

![Balena Etcher download button](Images/balena_download.png)

Now plug in your USB drive and you're ready to use etcher.

<div id='useetcher'/>

### Using Etcher

To open Etcher, simply run the .exe you just downloaded (probably in your downloads). (If you don't see the .exe at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .exe)

To run the .exe you can either double click it (left click). Or right click it and select run as admin.(NOTE: Running as admin may fix some issues when running Etcher so it is generally suggested to use this method) This should open Etcher.

Now that Etcher is open you should see an big button on the left saying "Flash from file". Click that button and select the Fedora Linux ISO that you downloaded in [Prep. Shopping List](#shopping_list). (probably in your downloads)

![Balena Etcher Flash Button](Images/balena_image_button.png)

Once you have your ISO selected make sure you have your USB drive selected. To do this, click the "select drive" button and pick your USB drive.

![Balena Etcher Select Target Button](Images/balena_Select_target_button.png)

Make sure everything is correct and if it is, click the big flash button and let it do it's thing.

![Balena Etcher Flash Button](Images/balena_flash_button.png)

Let it finish and when it does, you're ready to use your USB. No need to un-plug it as we'll be using it in [Step 2.](#step2)


<div id='o2rufus'/>

## Option 2. Rufus

Rufus creates a bootable install of linux (or whatever os you chose). However, you will only be able to boot to that single ISO or image that's burned to that USB drive.

<div id='dlrufus'/>

### Downloading Rufus

Download Link: https://rufus.ie/

Scroll down a bit until you see the download section. You'll want the one with p.exe at the end. This signifies it's the portable version. We'll be using the portable version as it skips the need to install.

![Rufus download button](Images/rufus_download.png)

Now plug in your USB drive and you're ready to use Rufus.

<div id='userufus'/>

### Using Rufus

To open Rufus, simply run the .exe you just downloaded (probably in your downloads). (If you don't see the .exe at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .exe)

To run the .exe you can either double click it (left click). Or right click it and select run as admin.(NOTE: Running as admin may fix some issues when running Rufus so it is generally suggested to use this method) When it asks you if you want to check for updates click no. This should open Rufus.

Now that Rufus is open it should automatically detect your USB drive. If not, click the little down arrow on the right under "Devices" and choose the correct one.

![Rufus Device Arrow](Images/rufus_drive_button.png)

Now that your USB drive is selected you can chose the ISO that rufus will install. To do this, simply click the "SELECT" button, then find your ISO (probably in your downloads).

![Rufus Select Button](Images/rufus_select_button.png)

Once your ISO has been selected you can click the "START" button at the bottom for it to start writing your Linux ISO to your USB drive.

#### NOTE: If you want to actually install linux to this USB drive you can move the "Persistent partition size" slider all the way to the right. This will allow that space to be installed to, however this guide doesn't cover that.

![Rufus Start Button](Images/rufus_start_button.png)

Let it finish doing it's thing and when it's done you can close Rufus. No need to un-plug your USB drive as we'll be using it in [Step 2.](#step2)

<div id='o3ventoy'/>

## Option 3. Ventoy

#### NOTE: Ventoy creates a [bootloader](#Term_Bootloader) on your USB drive that will allow you to select whatever ISO you want (as long as it's on the USB drive). It also allows you to quickly chose between whatever distro's ISO you have on your ventoy

<div id='dlventoy'/>

### Downloading Ventoy

Download link: https://github.com/ventoy/Ventoy/releases

You'll want the one with windows.zip at the end. As ventoy gets updated the verison number will change. As of making this guide it's 1.0.94.

![Ventoy Download Button](Images/ventoy_download.png)

<div id='suventoy'/>

### Setting up Ventoy

There's a more informative guide on how to do this here: https://www.ventoy.net/en/doc_start.html

#### NOTE: The above guide doesn't cover things super in-depth so if you're a total novice it may be intimidating.


First, unzip the .zip that you downloaded. To do this open file explorer and find the .zip file you just downloaded (probably in your downloads). Right click on the file and click extract here. This will make a folder named the same as the zip file.

(Optionally If you want to be organized i suggest putting the ventoy folder in your documents folder for easy access. Now it won't get lost in your downloads.) (If you don't see the .zip at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .zip)

Now, plug in your USB drive and you're ready to use ventoy.

<div id='useventoy'/>

### Using Ventoy

#### NOTE: If you've already installed ventoy on your USB you can skip to [Putting Your ISO on your USB](#isotoventoy).

First, run the file named "Ventoy2Disk.exe". This will be in that folder you just extracted. (If you don't see the .exe at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .exe)

You can either double click it(left click). Or right click it and select run as admin.(NOTE: Running as admin may fix some issues when running ventoy so it is generally suggested to use this method) This should open the ventoy tool.

Now that you have ventoy open we're ready to install it to your USB. To do this, look under device and make sure you have the correct drive selected. This should be your USB that you're installing to.

![Ventoy Drive Selection](Images/ventoy_drive_Selected.png)

If it's not already shown there click the little down arrow on the right side of the device box and select your USB drive from the drop down.

Once you have your USB drive selected, click Install and let it do it's thing.

![Ventoy Install Button](Images/ventoy_install_button.png)

When it's done the boxes "Ventoy in Package" and "Ventoy in Device" should match

![Ventoy Completed Screen](Images/ventoy_completed.png)

<div id='isotoventoy'/>

### Putting Your ISO on your USB

Putting your ISO on your USB is quite simple. Open file explorer and go to where you downloaded your Fedora Linux ISO (probably in your downloads). Then, on the left find where your USB drive is. If there are two partitions or two USB drives showing up, you'll want the larger one, or the one NOT named "VTOYEFI". (There may be two showing up as one is the ventoy partition (VTOYEFI) which is what boots up so you can select what iso you want to use. The other, larger one, is where you will store your ISO's. The best part is you can add as many as you can fit on your USB.)

Now that you've located your USB drive, simply drag and drop the ISO from your downloads to your USB. {idk if it asks to move or copy but here's this in case. "if it asks you to move or copy, selecting copy will leave a copy behind in case you want it for later."}

You now have your ISO on your USB and you're ready for [Step 2.](#step2) No need to un-plug as we'll be using it shortly.

<div id='step2'/>

# Step 2. Booting into Linux

Booting into Linux is the final hurdle before you can start learning about it, and using it.

#### NOTE: Nothing you do will get saved in the live environment. (This will be explained later in [The Live Environment](#liveenv))

<div id='bios'/>

## The BIOS

The BIOS is like integrated software on the motherboard that lets you change some special settings about your computer.

The BIOS is also where you can change what drive your pc uses to boot. We'll be going into it to tell your pc to boot off your USB drive with Linux on it.

<div id='tobios'/>

### Getting to your BIOS

To get to your BIOS you will need to hold a key while your computer is booting.

Some computers will tell you what key leads to the bios when they boot. Most commonly it will be the "delete" or del key on more modern systems. Other common keys would be f2, f12, f10, or f1. You can hold them all at once if you're really not sure but that's not reccomended.

 (On laptops these may be on your number keys and you might have to hold fn as well)

<div id='navbios'/>

### Navigating your BIOS

Navigation or more simply moving around in your BIOS is done mostly through arrow keys and the enter key, though some allow you to use your mouse.

<div id='navventoy'/>

## Navigating Ventoy

#### NOTE: If you used [Rufus](#o2rufus) or [Balena Etcher](#o1etcher) you can skip to [The Live Environment](#liveenv)

Navigating Ventoy is pretty simple and not too different from how most Linux distros boot when installed.

<div id='liveenv'/>

## The Live Environment

The live environment is where you can use fully featured linux without having to install. As mentioned before nothing you do here will get saved, you'll have to install for that. However, for the purposes of trying out linux and getting farmiliar with it, the live environment is a safe way to do so without making any commitments.

*Most* linux installers boot into a live environment by default, simply close out of the installer or click the "Try Nix" button.

<div id='step3'/>

# Step 3. Learning Linux


<div id='step4'/>

# Step 4.

