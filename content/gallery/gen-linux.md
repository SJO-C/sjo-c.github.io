---
# [str] Title of the project. This is also visible when hovering over a gallery item.
title: "General Linux"
# [str] Optional subtitle of the project. 
#   Functions as an additional explanation when hovering over a gallery item (comment out the following line).
subtitle: "Ask me about my General Linux Usage"
# [date] Project publication date.
#   Changes order: The newest item will be displayed first in the gallery. 
#   Just like Hugo's natural ordering, this is anti-chronological.
#   You can use 'weight' to order (primarily) for more control (sometimes it makes sense to put old items before new ones).
#   The specifics are documented here: https://gohugo.io/templates/lists/#order-content
date: "2024-09-16T18:52:34+01:00"
# [str] Gallery image file from the assets directory. 
image: "images/Tux.png"
# [str] Alternative (image) description.
alt: "Tux, the Linux Penguin."
# [css] Optional background color of the gallery item (if omitted, will use theme's fallback).
color: "#fff"
# [css] Optional gallery item hover color (if omitted, will use theme's fallback).
#hoverColor: "#fff"
# [map] Configure github specific options here:
# github: 
    # [str] Repo is a combination of "<user_or_org>/<repository_name>"
    # repo: "SJO-C/gen-linux"
    # [bool] Show repository information such project language below the buttons.
    # showInfo: true
    # showButtons: true
# [map] Optionally configure terminal to be displayed when opening up the gallery item:
#   Example (set "useTermynal" to true in config.yaml and comment out to test it):
# terminal:
    # lines:
    # - type: input
    #   data: hugo mod get -u github.com/hugo-mods/lazyimg 
    #   wait: 1250
    # - type: progress
    #   data: 100
    #   wait: 200
    # - data: ✓ Done.
    #   wait: 75
    # - data: exit
    #   wait: 75
# buttons:
#   - i18n: view # i18n key (see i18n directory, see https://gohugo.io/functions/i18n/)
#     icon: view # optional: use an icon from icons.yaml
#     newTab: false # optional: controls if url should be opened in new tab
#     url: ""
#   - i18n: code 
#     icon: code
#     url: ""
# [bool] Draft mode will decide if file will be published to 'public/' directory.
draft: false
---
I first got involved in the Linux Scene c.2012, with the initial Raspberry Pi model B, which ran the Raspbian OS (now known as Raspberry Pi OS) as its recommended OS.  As a consequence, I began to learn the ropes (so to speak) of Debian(based) Linux from around age 10.  From that point, I mainly used Debian & Ubuntu (and its derivatives) on my Pi & in Virtual Box on the Family Computer.  However, it wasn't until I reached Sixth Form that I began to experiment with non-Debian (dpkg/apt) derived Distros, owing to lack of familiarity with other package managers. In 2019, I tried Fedora, necessitating the learning of the Dandified Yum (DNF) package manager whilst also getting use to a system with SELinux enforcement. 

It was during this time, pre-COVID, that I started to use NixOS - as a consequence of Fubar-ing an Ubuntu Install.  I managed to break the Ubuntu install to the point of Kernel Panics on Boot, after attempting to upgrade the Kernel Version, whilst using an OpenZFS file system which, it transpired, was reliant on a DKMS module driver, which I hadn't realised I had to update.  As a consequence, I clean installed NixOS over the Ubuntu Install, as I was not nearly skilled enough to try to recover the Ubuntu Install itself.

Since then, I have begun to experiment with using Docker (And Docker Compose), Cloudflare's Tunnels, Hugo (which generates this site), TrueNAS Scale & also start to try using BSDs, mainly FreeBSD as well as attempt (without success) to install Gentoo Linux in a VM.  However, I'll be first to admit that I am still very much in the early stages of learning all of these technologies.