---
layout: post
current: post
cover: 'assets/images/rust.png'
navigation: True
title: Rust gets included in the next linux kernel
date: 2022-09-30 10:18:00
tags: posts-2022
class: post-template
subclass: 'post'
author: Avinash
---

## Introduction : 
Rust will be utilized in the next version of the Linux kernel, according to Linux Torvalds, the operating system's founder. Rust inclusion in Linux kernel development was a topic of discussion for several years before it was eventually settled.

# What exactly is Rust ?

Rust is a static compiled language which focuses on performance, memory safety without the use of garbage collectors. Rust has been adapted by several major companies such as Amazon, Discord, Meta, Google and even Microsoft.Rust contains a safe mode where the compiler will check for errors, but it comes with a downside - it is considered a bit restrictive. And for those, who doesn’t like it, they can enable the unsafe mode where this restriction is removed, but then the correctness of the program is to be done by the programmer’s end.

# So what’s gonna happen when Rust gets included in Linux ?

Rust is now only being used to write driver code, but it will eventually make an appearance in the kernel as well. Switching to Rust has the previously mentioned benefit of fewer coding memory errors thanks to its "Safe mode." Additionally, writing driver programs becomes somewhat simpler. There is a long way to go; let's wait and see what happens. :-)