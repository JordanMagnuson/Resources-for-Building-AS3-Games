# Help and resources for building AS3 Flash games post-2020

This repository contains help and resources for building ActionScript 3 Flash games in the post-2020 "death of Flash" era.

This guide can be used as a general referrence for getting ActionScript 3 code compiling, but also has specific instructions for the following IDEs and frameworks:
- FlashDevelop
- FlashPunk

Have additional tips, or guides for other IDEs or frameworks? Please contribute!

Have old AS3 games lying around? Please consider releasing the source code if possible, to aid Flash game preservation efforts!

## Setting up FlashDevelop for AS3 post-2020

In order to start building Flash games we need to get FlashDevelop (a free AS3 code editor and IDE) set up with Flex SDK and debug Flash player. 

There are a few hiccups when it comes to doing this post-2020, but it is still possible.

We will be using this guide as a basis for setting up FlashDevelop: [FlashPunk Tutorial: Setting Up FlashDevelop](http://useflashpunk.net/getting-started/setting-up-flashdevelop.html)

(Finding dead links? Try the Wayback Machine: https://web.archive.org/)


## 1. Install Flash Develop

First of all, make sure you have Java 32-bit installed on your system: [https://www.java.com/en/download/manual.jsp](https://www.java.com/en/download/manual.jsp)

![](https://i.imgur.com/z1gbRx6.png)

Then download and install the latest version of Flash Develop from [here](https://www.flashdevelop.org/). (Windows binary also included in this repository.)

![](https://i.imgur.com/8giRPzW.png)

![](https://i.imgur.com/gCS2u3I.png)

Windows and/or Chrome may try to block this download. You may need to right click and “save file as”, then tell Chrome that you want to keep the file. 


Run the installer to complete installation.

You can ignore the installer warning about needing the Flash Active-X plugin for IE. 


## 2. Download the Flex SDK

Flex SDK is what allows you to actually compile AS3 code into an SWF or AIR file that you can run with a Flash player.

It’s somewhat hard to get Flex SDK working these days using old sources. Specifically because the Apache Flex SDK installers no longer work. In theory you should still be able to get things set up by using the zip downloads provided by [Apache Flex](http://flex.apache.org/download-binaries.html) and/or [Harman](https://airsdk.harman.com/download), but it can be tricky.

I’ve packaged a working binary release of Apache Flex SDK 4.16.1 for Windows which is included in this repository.

Unzip the contents of that zip into a root folder like c:\Flex


## 3. Configure Flash Develop

Go to Tools > Program Settings > AS3Context and add the Flex SDK to installed SDKs:

![](https://i.imgur.com/VJaBqUt.png)

![](https://i.imgur.com/em40xL5.png)

Choose the folder where you put the Flex SDK:

![](https://i.imgur.com/8ynwxts.png)

Next, set the FlashViewer path to “flashplayer_32_sa_debug.exe” contained in the Flex SDK folder:

![](https://i.imgur.com/3RfhvHB.png)


## 4. Hello World

Continue with the Hello World test from [FlashPunk Tutorial: Setting Up FlashDevelop](http://useflashpunk.net/getting-started/setting-up-flashdevelop.html#hello-world) (step 2 on that page).

You should see the flash player window pop up (with nothing in it), and “Hello World!” displayed in the debug console area:

![](https://i.imgur.com/IxGNN8U.png)

## 5. Installing FlashPunk

“FlashPunk is an ActionScript 3 library, meaning it is not a piece of software or single program, but rather a huge collection of ActionScript 3 (.as) files that contain helpful code for setting up your games, rendering different types of graphics, resolving in-game collisions between objects, and much, much more. In order to use it, you’re going to have to download the library and import it into your projects.”

Download the FlashPunk 1.7.2 source code zip from [https://github.com/useflashpunk/FlashPunk/releases/tag/v1.7.2](https://github.com/useflashpunk/FlashPunk/releases/tag/v1.7.2)

(Also included in this repository)

Drag the “net” folder from that zip into your AS3 project’s src folder:

![](https://i.imgur.com/PHjxslM.png)


Follow the directions at [http://useflashpunk.net/basic/flashpunk-basics.html](http://useflashpunk.net/basic/flashpunk-basics.html) to change your /src/Main.as file in order to start testing out FlashPunk.

Congratulations: "Flash is dead," and you are now ready to make your first Flash game using AS3 and FlashPunk. :-)
