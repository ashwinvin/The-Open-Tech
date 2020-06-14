---
layout: single
title: "Use your Raspberry-Pi to block Ads"
date: "2020-06-13 22:33:39 +0530"
header:
      image: "/assets/images/pi_hole6.png"
      teaser: "/assets/images/pi_hole6.png"
---

The Pi-hole is a DNS sinkhole that protects your devices from unwanted content, without
installing any client-side software. If explained with simpler terms, it essentially means an
ad blocker, But unlike conventional  Ad blockers which run on our browsers and block ads
only for us, Pi-hole can block for  **all**   devices on your network and all you need is a
**Raspberry-Pi**  connected to your router.

It can also run using docker. Check here: <https://github.com/pi-hole/docker-pi-hole>
{: .notice  --info}

It blocks more **_1.6 million_**  ad serving domains before they even reach your computer
:smiley:.

## Installing Pi-Hole

Installing Pi-hole in raspberry is ridiculously easy.
```bash
curl -sSL https://install.pi-hole.net | bash
```
 Run the above command in terminal and it will launch the interactive installer. Answer the
questions and Pi-hole will be installed.

## Configuring devices to use Pi-Hole

To individually configure your devices to use Pi-hole.

1,  Go to settings
2,  Find Network options
3,  Find DNS Settings
4,  Set DNS to the IP address of the Raspberry-Pi

##### Finding IP address of Raspberry-Pi
To find IP address of your Raspberry-Pi. Login and run
```bash
hostname -I | awk '{print $1}'
```
This will give you the IP address of your raspberry

Now you've setup your Pi-hole. Its time for me to start writing another blog and you to start
browsing the internet **Ad-Free**  :smiley:. Until then, BYE. :wave:
