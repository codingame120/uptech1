---
title: "How to Play Music in Termux"
date: 2021-10-20T00:29:38+02:00
draft: false

description: "If you want to learn how to play music and other audio files on your phone with TERMUX, you are on the right place."

tags: ["Termux", "phone", "Music", "Audio"]
categories: ["Termux"]

hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: "/posts/how-to-play/img/play.jpg"
featuredImagePreview: "/posts/how-to-play/img/play.jpg"

toc:
  enable: true
math:
  enable: false
lightgallery: false
license: ""
---

<br/>
<br/>

## Introduction

Why would you want to play audio files and music in termux terminal on your phone? Well if nothing else then because is fun... <br/> There are more ways ( Programs for play music and audio files in termux ). In this article, we will look for one who calls **_play-audio_**.

<br/>

First as good practice we need to run:

```
pkg update && pkg upgrade
```

commands to update and upgrade our repositories.

## Install play-audio

After that just simple run:

```
pkg install play-audio
```

When play-audio is instaled navigate to the music directory.
<br/>You can do that by command:

`pwd`

stands for Print Working Directory, to see where you are.
<br/>And command:

`cd`

stands for Change Directory, to navigate through directories.
<br/>And you can use command:

`ls`

stands for List, which will list all files in a directory.

## Play Audio Files

When you get to directory where is your music ( audio file ) run:

```
play-audio [ 'name of the file' ]
```

<br/>
It is simple as that, now you can play music and audio files on your phone using termux terminal.

## Watch Video Example

You can watch and video example:

{{< youtube 2laQXniX2oY >}}
