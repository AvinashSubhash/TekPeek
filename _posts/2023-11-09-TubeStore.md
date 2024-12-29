---
layout: post
current: post
cover: 'assets/images/tubestore.png'
navigation: True
title: TubeStore - Free Youtube Storage
date: 2023-11-09 10:18:00
tags: [posts-2023,tools]
class: post-template
subclass: 'post'
author: Avinash
---

# Cloud Storage
Cloud storage subscriptions are in high demand due to the exponential growth of data generation. With the advent of digital technology, data production has increased tremendously, leading to a need for more storage capacity. You may have experienced a situation where your Google Drive or other cloud storage shows a warning of reaching its limits. To get more storage, you need to pay more, and this can be quite expensive.

Within these vast amounts of data, we often have some items that are not accessed frequently, but that we still need for possible future use or as a memory to keep with ourselves. However, you may not have considered YouTube's storage and its growing number of content creators. YouTube handles a significant amount of data daily, mostly videos from these content creators, and it doesn't charge any money for that. What if we could use that storage for our data too? Of course, we're not trying to steal YouTube's storage, but merely suggesting an idea of how we could make use of it.

# What is TubeStore ?
TubeStore is a tool written in python which can be used to convert any data into a video format, and revert back to the original final without any loss.

# How does it work ?
As we all know, data comes in different formats, but all these formats are stored in 0s and 1s at the end. This is where this tool comes in. It converts all the data to 0s and 1s and creates image frames where each pixel has a value of 0 or 1. This way, if we arrange the binary numbers in the same sequence, we can represent the data in a set of images/frames - thus creating a video.

Using this method, we can save our data in the form of videos, which is a novel approach to data storage. The process is simple, and it is an excellent way to save data that is not accessed frequently. It is also a great way to keep a memory that we need to keep with ourselves.

This tool is useful for taking binary values and shaping them into a different form, but there are two disadvantages that we need to keep in mind. Firstly, the size of the videos generated can be up to 4 times the size of the original file. This means that you need to have a lot of storage space to accommodate the videos that are generated. Secondly, we need a lot of RAM and processing power to convert large files to videos. This can be a significant challenge, especially when dealing with large files.

Currently, while testing on Linux (Ubuntu 22.04), this tool can convert files up to 200 MB into videos. Beyond that, the RAM gets filled, and the program is killed by the system for safety reasons. However, this is still a significant milestone, and it shows that there is potential for further development of this tool.

# Conclusion
In conclusion, the idea of using YouTube's storage for our data is a novel approach to data storage. It is an excellent way to save data that is not accessed frequently, and it is also a great way to keep a memory that we need to keep with ourselves. However, we need to keep in mind the two disadvantages of this tool, namely the large size of the videos generated and the need for a lot of RAM and processing power. Nonetheless, this is still an exciting development, and it is worth exploring further to see how it can be improved.

Also, it has been noticed that converting png files causes corruption while reverting back.

The github repository can be accessed here - https://github.com/AvinashSubhash/TubeStore