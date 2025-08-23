---
layout: post
title: "FreeXR status update #1"
author: "ThatOSDeveloper"
categories: FreeXR Linux
tags: [development]
---

FreeXR has currently had a few things done, first of all we released the (now patched, at least we think) root exploit for the Meta Quest 3(s), once again, PLEASE run this command with adb to disable updates on your device (YOU WILL LOSE THE ABILITY TO ROOT IF YOU UPDATE!) the root IS NOT PERMANENT! AND IS LOST ONCE YOU REBOOT! PLEASE DO NOT CLICK INSTALL IF YOU HAVE MAGISK!

```bash
adb shell pm disable-user --user 0 com.oculus.updater # Disable updates on META Quest Devices
```

This is needed to disable updates PLEASE RUN IT! Anyways, here are the actual updates (just gonna bullet point them, im a bit lazy)

1. The exploit for the Quest 3(s) has been released [here](https://github.com/FreeXR/eureka_panther-adreno-gpu-exploit-1)
2. We have a list of exploits [listed here](https://github.com/FreeXR/exploits)
3. We also have a list of safe things you can do with root (will not brick the device) [listed here](https://github.com/FreeXR/safe-root-things)
4. We have a Magisk fork you can [find it here](https://github.com/FreeXR/Magisk-FreeXR)

Some more info on the Quest 3(s) exploit, please for the love of God read the readme file, if you do not, you will brick the system. The exploit has a CLI/TUI for picking what you want to do, your options are only disabling SELinux (useful for a few small things), getting only root, doing both (Disabling SELinux and getting root, you need to disable SELinux to use Root afaik, or be able to use root for anything useful), or install Magisk (will not do a perma install, just the magisk manager)

Once you finally have it setup, please do **NOT** modify /system, or any other critical file, you **WILL** brick your system! The root is temporary! But changes are not! Any changes made **WILL BRICK YOUR SYSTEM ALL OF THE TIME** unless otherwise noted in the safe root things! Once we get a permanent root it WILL be safe.
