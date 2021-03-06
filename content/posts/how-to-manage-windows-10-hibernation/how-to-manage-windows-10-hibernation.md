---
title: "How to Manage Windows 10 Hibernation"
date: 2022-01-21T10:07:36+01:00
draft: false

author: ""
authorLink: ""
description: "How to control hibernation in Windows 10, how to minimize the size of the hibernation file andmanipulate with a fast boot."

tags: 
  - Windows 10

categories: 
  - Windows 

hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: "/posts/how-to-manage-windows-10-hibernation/img/hibernate.webp"
featuredImagePreview: "/posts/how-to-manage-windows-10-hibernation/img/hibernate.webp"

toc:
  enable: true
math:
  enable: false
lightgallery: false
license: ""
  
---
<br>

If you've been thinking about ways you can optimize your Windows 10 operating system, hibernation management is one of them. 
You can turn on or off hibernation depending on desire and need, but you can also reduce the disk space that hibernation requires, which is especially convenient if you have a disk with less space. 
Hibernate uses as much disk space as you have RAM. 

You don't need any special third-party tools or applications, everything can be easily done through Command Prompt (CMD).Press the Windows button and type: `cmd`. Open Command Prompt (CMD) as administrator.


You can check the size of the hibernation file by typing the following command:`dir c:\hiberfil.sys /ah`

<br>

## Mange Hibernation

<br>

Let's have a look at how to enable or disable hibernation. lower the size of the hibernation file or change the desired file size.

* To disable hibernation, type: `powercfg/h off`

* To enable hibernation, type: `powercfg/h on`

* If you want to use Windows Fast Startup but not hibernate, change the hibernation file type to reduced:`powercfg/h/type reduced`, which takes up less disk space than a regular hibernation file. To restore the hibernation file, change the /type parameter to full: `powercfg/h/type full`

* Turn on hibernation and specify the size of the hibernation file as a percentage of installed RAM using this command: `powercfg/h/size nn` Enter a number between 40 and 100 in place of nn. Avoid making this amount smaller, because you will be unable to use the hibernate file.


<br>

## Conclusion
<br>

It was a brief and succinct demonstration of how to control hibernation to optimize Windows 10 and make the most of this benefit while also balancing limited space and desired fast boot.