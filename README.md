# Step by step guide to your first time in Linux!

### This is an in-depth guide you through your first time using linux from being a complete beginner with computers.

### Contents
1. [Prep. Shopping list, terms, and imformation](#shopping_list)
    1. [Some important terms](#terms)
2. [Step 1. Getting Linux on your USB](#step1)
    1. [Option 1. Ventoy](#o1ventoy)
        1. [Downloading Ventoy](#dlventoy)
        2. [Setting up Ventoy](#suventoy)
    1. [Option 2. Balena Etcher](#o2balena)
        1. [Downloading Balena](#dlbalena)

<div id='shopping_list'/>

# Prep. Shopping List, terms and information

### These are the things that you'll need to follow along with this guide. You probably already have these items laying around!

1. Usb drive with at least ~8GB or more. (you can probably get away with less, around 4GB, but you'll be pretty limited as to what you can do)

2. A pc running windows with a usb port. (while you *can* do this on an intel based mac but it's not covered in this guide)

3. A Linux ISO.  For this guide we'll be using NixOS. https://nixos.org/download

Scroll down until you find this section and click Download. (We'll be using the Plasma version as it's more Windows like and should be more farmiliar to you. You may choose the gnome version if you'd like but that's not covered in this guide)

![NixOS download button](NixOS_download.png)

4. A tool to get the linux ISO on to the usb. (This will be covered in Step 1.)

<div id='terms'/>

### Some important terms

- ISO: An ISO, also known as an *image*, is an archive, usually as a backup of optical media like CD's. In this case it's used to distribute a copy of linux. Not too different from physical install disks from back in the day.

- Distro: Distro, or distribution refers to the distribution of linux as there are many to chose from. Think of it like a supermarket. Target, Walmart, Whole Foods, Aldi, would be the distributions or different choices under the umbrella term of "supermarket".

- Linux: Linux refers to the Kernel that tells everything else what to do.
For more context (and an inside joke with the linux community) see this copypasta https://stallman-copypasta.github.io/

- Kernel: The kernel is a computer program at the core of a computer that communicates between programs and things like your mouse and keyboard and tells everything what to do.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Kernel_%28operating_system%29

- DE: DE is short for Desktop Environment. A Desktop Environment is a bundle of programs that allow you to interact with your computer. Think of your task bar and start menu. That's all part of the DE. In the case of this guide we'll be using one called Plasma by KDE. gnome is also a different DE.
For more info see this wikipedia article https://en.wikipedia.org/wiki/Desktop_environment

- WM: WM is short for Window Manager. A Window Manager is software that, as the name implies, manages your windows (the little boxes of programs that show up on your screen like google). The window manager mainly handles their position and how they move around, though that's a gross oversimplification.
afor more info see this wikipedia article https://en.wikipedia.org/wiki/Window_manager

<div id='step1'/>

# Step 1. Getting Linux on your USB

## For putting Linux on the USB we have two options. Doing either of which will remove everything on your USB drive so make sure you have everything backed up.

<div id='o1ventoy'/>

## Option 1. Ventoy (We'll be using this option for the rest of the guide.)

Ventoy creates a bootable USB drive that will allow you to select whatever ISO you want (as long as it's on the USB drive). Using ventoy to boot into Linux will be covered in Step 3.

<div id='dlventoy'/>

### Downloading Ventoy

For ventoy you have 2 ways to download. Both of which give you the same thing so you can pick one way or the other.

Download link 1: https://www.ventoy.net/en/download.html

You'll want the one with windows.zip at the end. As ventoy gets updated the verison number will change. As of making this guide it's 1.0.94.

![Ventoy Download Button1(ventoy_download1.png)

Download link 2: https://github.com/ventoy/Ventoy/releases

You'll want the one with windows.zip at the end. As ventoy gets updated the verison number will change. As of making this guide it's 1.0.94.

![Ventoy Download Button2(ventoy_download2.png)

<div id='suventoy'/>

### Setting up Ventoy

There's a more informative guide on how to do this here: https://www.ventoy.net/en/doc_start.html

#### NOTE: The above guide doesn't cover things super in-depth so if you're a total novice it may be intimidating.


First, unzip the .zip that you downloaded. (If you don't see the .zip at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .zip)

To do this open file explorer and find the .zip file you just downloaded (probably in your downloads). Right click on the file and click extract here. This will make a folder named the same as the zip file. (Optionally If you want to be organized i suggest putting the ventoy folder in your documents folder for easy access. Now it won't get lost in your downloads.)

Now, plug in your USB drive.

Next, run the file named "Ventoy2Disk.exe". This will be in that folder you just extracted. (If you don't see the .exe at the end don't worry. Go to the view tab at the top of file explorer, and click the "Show file extensions" check box. You should now be able to see the .exe)

You can either double click it(left click). Or right click it and select run as admin.(NOTE: Running as admin may fix some issues when running ventoy so it is generally suggested to use this method) This should open the ventoy tool.

<div id='o2balena'/>

## Option 2. Balena Etcher

Balena Etcher etches or burns the image on to that USB. Similar to burning a CD back in the day. This means that you will only be able to boot to that single ISO or image that's burned to that USB drive. Though much more limited this method is alot simpler and will serve it's purpose for this guide.

<div id='dlbalena'/>

### Downloading Balena Etcher

Doanload link: https://etcher.balena.io/#download-etcher

{insert download image here. i'll worry about this later since the guide doesn't use this option.}


<div id='step2'/>

# Step 2. 



<div id='step3'/>

# Step 3. 
