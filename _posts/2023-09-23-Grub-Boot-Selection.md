---
layout: post
current: post
cover: 'assets/images/grub.jpg'
navigation: True
title: How to Make GRUB Remember Your Last Selection on Boot
date: 2023-09-23 10:18:00
tags: posts-2023
class: post-template
subclass: 'post'
author: Avinash
---

## Introduction :
GRUB is an essential part of most Linux systems, responsible for managing the boot process and allowing you to choose which operating system to boot into when you start your computer. By default, GRUB usually selects the first entry in the boot menu. However, many users prefer to make GRUB remember their last selection to streamline the boot process. In this tutorial, we'll walk you through the steps to configure GRUB to remember its last selection on boot.

## Step 1: Opening the GRUB Configuration File
The first step is to open the GRUB configuration file, which is located at /etc/default/grub. You'll need superuser (root) privileges to edit this file, so use a text editor like 'nano' or 'vi' with the 'sudo' command

```sudo nano /etc/default/grub```

## Step 2: Setting the Value of GRUB_DEFAULT to 'saved'
Inside the configuration file, you'll find various GRUB settings. Look for the GRUB_DEFAULT variable. By default, it may be set to a numerical value, such as 0 for the first menu entry. Change it to:

```GRUB_DEFAULT=saved```

## Step 3: Setting the Value of GRUB_SAVEDEFAULT to 'true'
Next, find the GRUB_SAVEDEFAULT variable in the configuration file. If it's not present, you can add it. Set its value to 'true'

```GRUB_SAVEDEFAULT=true```

## Step 4: Saving the File
After making these changes, save the GRUB configuration file and exit your text editor. In 'nano,' you can do this by pressing Ctrl + O to save and Ctrl + X to exit. In 'vi,' you can save by pressing Esc, then typing :wq, and hitting Enter.

## Step 5: Generate the GRUB Configuration File
The final step is to generate the GRUB configuration file using the grub-mkconfig command. This command will take the changes you made to /etc/default/grub and apply them to the actual GRUB configuration

```sudo grub-mkconfig -o /boot/grub/grub.cfg```

This command rebuilds the GRUB configuration file located at /boot/grub/grub.cfg. After running this command, GRUB will remember your last selection and use it as the default entry during the next boot.

## Conclusion

Configuring GRUB to remember its last selection on boot can be a time-saver and a convenient feature for those who frequently switch between different operating systems or boot options. By following the steps outlined in this guide, you can easily make GRUB remember your last selection and improve your overall boot experience on your Linux system.