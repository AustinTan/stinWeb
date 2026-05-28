---
title: Reduce your game size for free using CompactGUI
description: "No more space for a new 100gb game? Reduce your game size with CompactGUI, a free and open-sourced tool."
tags:
  - Utility
date: 2026-04-20T14:19:51.000Z
draft: true
categories:
  - Guide
slug: 0fa8178
author: "{name: Austin Tan Yong Hiok, link: null, email: null, avatar: null}"
weight: 0
lastmod: 2026-04-25T10:36:19.631857Z
comment: true
hiddenFromHomePage: false
hiddenFromSearch: false
hiddenFromRelated: false
hiddenFromFeed: false
repost:
  enable: false
  url:

---


<!--more-->
# Introduction
With the soaring prices of DRAM module, even the price of SSD is affected. With limited storage and huge game sizes, what are our options?

Meet CompactUI, a completely free and open-source tool. With CompactUI this you can reduce the game sizes around 20-30% with negligible performance impact.

In this guide I will introduce how to use this tool and some problem I’ve encountered while using it.

# Installation
Navigate to its [GitHub Repository](https://github.com/IridiumIO/CompactGUI/releases).

Find a stable version, preferably without beta.
Download **CompactGUI.exe**

Then just run **CompactGUI.exe**

# Using CompactGUI
After starting it, navigate to Home. Then, click add a folder and navigate to the game folder you want to compress. For instance, by default steam game is usually located in: `C:/Program Files/Steam/commonapp/downloaded/Counter-Strike: Global Offensive`

If you added a game from steam, it should automatically identify the game with its database. It will tell you the estimated file size saved with every compression ratio. Generally I find **XPRESS 8K** to have the best compression and performance balance. Anything above it have minimal impact on the size saved.

Another feature is its database, everytime you compressed a steam game. It will collect the information about the compression (i.e. how much size is saved) and upload it to the database to allow other users to see. All the information can be viewed at the Database page.

