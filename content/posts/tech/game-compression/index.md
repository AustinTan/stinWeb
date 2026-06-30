---
title: Reduce your game size for free using CompactGUI
description: "No more space for a new 100GB+ game? Reduce your game size with CompactGUI, a free and open-sourced tool."
keywords: 
  - game compression
  - CompactGUI guide
  - reduce ARK size
tags:
  - Utility
date: 2026-06-02T14:19:51.000Z
type: "posts"
draft: false
categories:
  - Tech
slug: reduce-your-game-size-for-free-using-compactgui
author: 
  name: Austin Tan Yong Hiok
  link: https://stinweb.com
  email: austin@stinweb.com
  avatar: null
weight: 0
lastmod: 2026-06-02T10:36:19.631857Z
comment: true
hiddenFromHomePage: false
hiddenFromSearch: false
hiddenFromRelated: false
hiddenFromFeed: false
repost:
  enable: false
  url:
featuredImage: 
featuredImagePreview: 
---


<!--more-->
## Prerequisite
>[!Attention]+
> -   OS: Windows 10 and above
> - Can only be used on game without ***DirectStorage API***

## What does it do?
It reduce file sizes of game with negligible performance impact using a Windows 10 feature (compact.exe).

### Example:
|Game|Original Size|Compressed Size|Saved Size|Mode|
|:--------:|:--------:|:--------:|:--------:|:--------:|
|Train Simulator Classic 2024|215GB|107GB|108GB / 50%|XPRESS4K|
|ARK: Survival Evolved|278GB|147GB|130GB / 47%|XPRESS4K|
|Assetto Corsa|189GB|71GB|118GB / 62%|LZX|
|ATLAS|136GB|78GB|58GB / 43%|XPRESS4K|
|God of War Ragnarök|174GB|134GB|41GB / 23%|XPRESS16K|
|Killing Floor 2|95GB|47GB|48GB / 51%|LZX|

Data is gathered from CompactUI's [database](https://github.com/IridiumIO/CompactGUI/blob/database/database.json).

## Installation

### Method 1: Direct Download
1. Navigate to its [GitHub Repository](https://github.com/IridiumIO/CompactGUI/releases).

2. Find a stable version, preferably without beta.
3. Download **CompactGUI.exe**

4. Then just run **CompactGUI.exe**

### Method 2: Windows Package Manager (CLI) 

1. Open CMD (Command Prompt) or PowerShell and run: 

```powershell
winget install CompactGUI
```

## How to use CompactGUI

### Compressing a game

After starting it, navigate to Home. Then, select a folder and navigate to the game folder you want to compress. For example, by default steam's game is usually located in: 

`C:/Program Files/Steam/commonapp/downloaded/ARK: Survival Evolved`

If you added a game from steam, it will tell you the estimated file size saved with every compression ratio. I just choose the one with the most size saved, because there's minimal performance impact anyways. Also if you experience any issues after compressing the game you can try ticking the **Skip file types likely to compress poorly**.

![CompactGUI Compression](CompactGUI-compression.webp)

### Game Compression Database

Another feature is its database, everytime you compressed a steam game. It will collect the information about the compression (i.e. how much size is saved) and upload it to the database to allow other users to see. All the information can be viewed at the Database page.

![CompactGUI Database](CompactGUI-database.webp)

### Watcher Feature

Adding a folder in the watcher lists means that the game will be re-compressed automatically after game updates. However, for this feature to be active `CompactGUI.exe` need to be running in the background.

![CompactGUI Watcher](CompactGUI-watcher.webp)

## Technical Explaination
