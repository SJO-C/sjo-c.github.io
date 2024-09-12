---
# [str] Title of the project. This is also visible when hovering over a gallery item.
title: "Student Futures Manifesto"
# [str] Optional subtitle of the project. 
#   Functions as an additional explanation when hovering over a gallery item (comment out the following line).
subtitle: "Ask me about the Student Futures Manifesto at the University of Lincoln's LALT & Students' Union."
# [date] Project publication date.
#   Changes order: The newest item will be displayed first in the gallery. 
#   Just like Hugo's natural ordering, this is anti-chronological.
#   You can use 'weight' to order (primarily) for more control (sometimes it makes sense to put old items before new ones).
#   The specifics are documented here: https://gohugo.io/templates/lists/#order-content
date: "2024-09-12T14:17:21+01:00"
# [str] Gallery image file from the assets directory. 
image: "images/sfm.jpeg"
# [str] Alternative (image) description.
alt: ""
# [css] Optional background color of the gallery item (if omitted, will use theme's fallback).
color: "#fff"
# [css] Optional gallery item hover color (if omitted, will use theme's fallback).
#hoverColor: "#fff"
# [map] Configure github specific options here:
# github: 
    # [str] Repo is a combination of "<user_or_org>/<repository_name>"
    # repo: "SJO-C/sfm"
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
buttons:
  - i18n: view # i18n key (see i18n directory, see https://gohugo.io/functions/i18n/)
    icon: view # optional: use an icon from icons.yaml
    newTab: true # optional: controls if url should be opened in new tab
    url: "https://www.lincoln.ac.uk/studentfuturesmanifesto/"
# [bool] Draft mode will decide if file will be published to 'public/' directory.
draft: true
---
In late 2022, I applied and was subsequently recruited as a student consultant to a joint project between my Institution's (University of Lincoln) [Lincoln Academy of Learning & Teaching](https://lalt.lincoln.ac.uk) and my Instituion's [Students' Union](https://lincolnsu.com/home)