---
title: "What Is Termux How to Install It and First Steps After Instalation"
date: 2021-10-20T00:48:32+02:00
draft: false

author: ""
authorLink: ""
description: "Everything you need to know about termux, including how to install it and what to do afterward.
TERMUX is an Android-based terminal emulator.
It means you can use a terminal on your phone to connect to the system, just like you can on Linux, Windows, or macOS."

tags:
  - Termux
  - Android

categories:
  - Termux

hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: "/posts/what-is-termux/img/termux.jpg"
featuredImagePreview: "/posts/what-is-termux/img/termux.jpg"

toc:
  enable: true
math:
  enable: false
lightgallery: false
license: ""
---

<br/>
<br/>

## Introduction To Termux

TERMUX is a terminal emulator for Android system.
It means that you can access to the system on your phone through a terminal like on Linux, Windows or macOS.
Since Android is built on Linux, Termux use Unix-like commands.

Unfortunately app is not available for iphone.

Those who use Linux and macOS will be familiar with commands.  
For those who use Windows will be little unfamiliar since CMD ( Command Prompt ) use different commands.  
But it's a great way to start Learn Unix-like commands and CLI  
( Command Line Interface ).  
Which is important if you want to do hacking and/or cybersecurity.

But Termux is not only hacking tool.

It can be useful for programmers since it can run python scripts and other programming language on your phone.  
So it can be useful and for those who want to learn programming.

You can do different things in TERMUX like send SMS send emails surfing Web or play music and audio files which you can read in our post: [How to play music in Termux.](https://www.uptech.cf/post/how-to-play-music-in-termux/)

There is no need to root access on your phone to use Termux.  
But if your phone have android older than 7.0 you will have to use Termux Legacy which don't have all functionality as Termux for newer version of Android.

## Installation

You can download Termux app on [Google play](https://play.google.com/store/apps/details?id=com.termux) or [F-Droid](https://f-droid.org/en/packages/com.termux/) store.

[<img src="/posts/what-is-termux/img/play.png">](https://play.google.com/store/apps/details?id=com.termux)
[<img src="/posts/what-is-termux/img/fdroid.png">](https://f-droid.org/en/packages/com.termux/)

<br/>

## What To Do After Installing Termux

So now when we have installed Termux on our phone. We need to do a couple of things.

- Update and upgrade repositories
- Install git
- Give Termux storage permission

### Update and upgrade repositories

Which can be done using commands:

```
pkg update && pkg upgrade
```

 <br/>
 
### Install git

Which can be done using `package manager` and `install command`:

```
pkg install git
```

<br/>

### Give Termux storage permission

Which can be done in two ways.

1.  First is to go to `settings>>apps>>termux>>permissions` and enable Termux to access storage.

    <p align="center">

    <img src="/posts/what-is-termux/img/tstorage1.jpg">

      </p>

2.  And second trough Termux command line. Which will work for **Android 6** and higher.

    Type command:

    ```
    termux-setup-storage
    ```

    You can check if Termux now have permission if `$HOME/STORAGE` folder is created.
    And if you have external storage (SD card) should check if app-private folder is created.
    Content of `$HOME/STORAGE` are symlinks to different storage folders.
    (e.g `~storage/music`)
    Standard folder for audio files.

<br/>

Now when you have set up Termux on your phone. You can start to explore play learn various different things with this interesting useful and very powerful app.

If you have any questions about Termux or suggestions, fell free to tell us in comments.
