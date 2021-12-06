---
title: "How to Install Metasploit in Termux?"
date: 2021-11-01T00:12:14+01:00
draft: false

author: ""
authorLink: ""
description: "This tutorial will demonstrate how to install Metasploit on the Termux terminal emulator for Android.You will find a complete guide with two methods covered."

tags:
  - Termux
  - Android
  - Metasploit
  - Hacking

categories:
  - Termux

hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: "/posts/how-to-install-metasploit-in-termux/img/metasploit.webp"
featuredImagePreview: "/posts/how-to-install-metasploit-in-termux/img/metasploit.webp"

toc:
  enable: true
math:
  enable: false
lightgallery: false
license: ""
---

<br/>
<br/>

## What Is Metasploit

<br/>
Metasploit is a free, open-source penetration testing framework.  
It is designed for use against a single computer or network, in contrast to other penetration testing tools such as nikto and cain and abel that target a network of computers.

This is done to reduce the time spent in scanning for a network, increasing the speed at which exploits can be found.  
The metasploit framework contains pre-configured plugins and exploits, although the user can also write their own.  
Metasploit is available for almost all operating systems, so it is very easy to get up and running with it.

All you need to do is download the metasploit framework, extract the package, and run it.

In this tutorial, we will be installing metasploit on the Android operating system.  
In order to install metasploit, you first need to download the metasploit framework package.  
There are two simple ways to install Metasploit on Termux.  
You may clone Metasploit and install it using git, or you can just install the Metasploit app using simple commands.

Let's start with a git-based method and then move on to a simpler method.

<br/>

But, as is generally good practice with thermux, let's update and upgrade repositories first.

Open Termux and run the following command to update your repositories.

```
pkg update && pkg upgrade -y
```

<br/>
<br/>

## How to Use Github to Install Metasploit in Termux

<br/>
Please carefully follow the steps below to install Metasploit in Termux via GitHub. And, after typing each command, you must wait for it to be executed.

After we've updated the Termux repository, we'll install some Metasploit prerequisites.

```
pkg install wget curl openssh git -y
```

We installed the following packages with the command above: Wget, Curl, Openssh, and git.

To install ncurses-utils, run the command below in your terminal.

```
apt install ncurses-utils
```

To download Metasploit, copy the following command and paste it into Termux.

```
wget https://raw.githubusercontent.com/gushmazuko/metasploit_in_termux/master/metasploit.sh
```

To make the file read, write, and executable, use the command below.

```
chmod +x metasploit.sh
```

To launch Metasploit, use the command below.

```
./metasploit.sh
```

If the previous command does not work, try the following command.

```
bash metasploit.sh
```

<br/>
<br/>

## Install Metasploit With Simple Command

<br/>
Run this command to install the unstable repository.

```
pkg install unstable-repo
```

To install Metasploit in Termux, use the command below.

```
pkg install metasploit
```

The installation procedure may take some time since Termux will automatically install other packages necessary to run Metasploit, such as Ruby, BisonFTP, and so on. Keep the Termux session open until the installation is finished.
<br/>

### How To Launch Metasploit

<br/>
After the installation is complete, you can now utilize the Termux to execute and use the Metasploit framework on your Android smartphone.

<br/>

To execute Metasploit in Termux, use the command below.

```
msfconsole
```

If this is not your first time launching Metasploit, ensure sure the PostgreSQL database is up and running. As a result, your Metasploit will run more smoothly and rapidly.

Before starting Metasploit, be sure to run Postgresql. You may use the following command to see if Postgresql is running or not.

```
pg_ctl -D $PREFIX/var/lib/Postgresql status
```

If Postgresql is already running, you will get the following output.

```
pg_ctl: server is running (PID: 9023 ) /data/data/com.termux/files/usr/bin/postgres "-D" "/data/data/com.termux/files/usr/var/lib/postgresql"
```

If Postgresql is not operating, you will get the following output.

```
pg_ctl: no server running
```

Let's look at how to get PostgreSQL up and running.

To start PostgreSQL, use the following command.

```
pg_ctl -D $PREFIX/var/lib/postgresql start
```

<br/>

That's it. Regardless of the approach you employed, you can now run Metasploit and begin exploring a wide range of possibilities. Happy hacking!
