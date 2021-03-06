---
layout: post
title: Nenuzhnix — my own Linux distro
---
Nenuzhnix (the name comes from the word "nenuzhno" meaning "useless") is my proof-of-concept Linux distro. It's idea was coming to my mind several times during 2014, I even made a small prototype. Now I'm going to describe what makes it so special.

This distro is going to be a mind-blowing mix of [Debian GNU/Linux](https://www.debian.org/), [OpenWrt](https://openwrt.org/) and [Aboriginal Linux](http://landley.net/aboriginal/). The main idea is using modern technologies while keeping things simple.
I will use the code and experience that I already have from my projects like Elk Linux (tiny embedded OS with Linux kernel) and Simplinux (a bunch of scripts to customize and build a small Linux based system) to achieve at least something with this new project.

Cool features:

* The Linux plague (systemd) will be replaced with a smaller init system (probably, something similar to OpenWrt init and [procd](http://wiki.openwrt.org/doc/techref/procd))
* Obsolete Xorg will be replaced with Wayland and Weston for GUI (Weston will be changed to something else later)
* Perl and Python workaround-scripts will be rewritten in pure sh, so I will not include the interpreters by default
* coreutils, util-linux and some other packages will be replaced with a single binary [toybox](http://landley.net/toybox/)
* dpkg will be replaced by opkg (compatible package manager from OpenWrt)
* dash will be the default shell instead of bash (bash also is not included by default)
* connman will replace NetworkManager

The aim of Nenuzhnix is to be a "yet another Linux distro" which is very small, understandable and simple, ideal for KISS principle fans.
