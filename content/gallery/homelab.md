---
# [str] Title of the project. This is also visible when hovering over a gallery item.
title: "Homelab"
# [str] Optional subtitle of the project. 
#   Functions as an additional explanation when hovering over a gallery item (comment out the following line).
# subtitle: ""
# [date] Project publication date.
#   Changes order: The newest item will be displayed first in the gallery. 
#   Just like Hugo's natural ordering, this is anti-chronological.
#   You can use 'weight' to order (primarily) for more control (sometimes it makes sense to put old items before new ones).
#   The specifics are documented here: https://gohugo.io/templates/lists/#order-content
date: "2025-02-05T16:28:48Z"
# [str] Gallery image file from the assets directory. 
image: "images/homelab.png"
# [str] Alternative (image) description.
alt: ""
# [css] Optional background color of the gallery item (if omitted, will use theme's fallback).
color: "#fff"
# [css] Optional gallery item hover color (if omitted, will use theme's fallback).
#hoverColor: "#fff"
# [map] Configure github specific options here:
# github: 
    # [str] Repo is a combination of "<user_or_org>/<repository_name>"
    # repo: "<username>/homelab"
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
# [bool] Draft mode will decide if file will be published to 'public/' directory.
draft: false
---
I have been 'home-labbing' since 2021 whilst studying.  The systems have been consistently small scale using Proxmox VE on small, low powered Intel N5105 Router Mini-PCs, and more recently on a 2nd Hand HP MicroServer Gen6.  Other components have/do included TP_Link 2.5GbE 5 Port Switch, an off-brand 2.5GbE Managed Switch, GLiNet Travel Router and a 16 Port 1GbE TP_Link Switch.

Currently, I self-host a set of VMs, one of which runs Docker, and one running OpenMediaVault - which serves as a local backup (Apple Time Machine) server for my MacBook.  The underlying Proxmox host (the HP Server) uses a ZFS filesystem and is rsync'd to a remote NAS running TrueNAS Scale.

The remote NAS runs a number of Docker Services including Plex, Jellyfin, Pinry (Self-hosted Pinterest Alternative), CraftyControl (Minecraft), Mealie (A food recipe manager), and PiHole for Ad-Blocking and Local DNS resolution.

The remote NAS also runs an instance of Home Assistant for my Parents to control their heating system owing to the poor quality of the system's native app.  

Since Oct. 2025, I have begun to try to learn Kubernetes (specifically K3S).  