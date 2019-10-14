# iBoot64helper

## Introduction

**iBoot64helper** is now an IDA loader!

Just copy *iBoot64helper.py* to your *~/.idapro/loaders/* (or your *IDA/loaders/*)
directory, launch IDA, and open a *decrypted* iBoot, iBEC, or SecureROM binary image.

<p align="center"><img src="screenshot-loader.png"/></p>

This aims to become an IDAPython utility to help with iBoot and SecureROM reverse
engineering. Currently it a) locates the image's proper loading address, b) rebases
the image, c) identifies functions based on common AArch64 function prologues, and
d) finds and renames some interesting functions.

As you can see in the screenshot below, 1920 functions
are recognized after running it on iBoot version 5540.0.129.

<p align="center"><img src="screenshot.png"/></p>

I will be adding features to it, identifying more functions, etc.

## References
[iOS RE Wiki](https://github.com/kpwn/iOSRE/blob/master/wiki/iBoot-RE.md)
