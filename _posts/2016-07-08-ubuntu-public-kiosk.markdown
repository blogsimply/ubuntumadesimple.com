---
layout: post
title:  "Public Kiosk in Ubuntu 16.04"
categories: Ubuntu Screencast
---

Sometimes you need to have a computer in a public place for people to use to quickly get online. Here's how you can accomplish this task quickly and easily with Ubuntu's guest mode. Simply follow the instructions in the video below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/tNA75HM5-Oo" frameborder="0" allowfullscreen></iframe>

##### List of commands:

```sudo mkdir /etc/guest-session
sudo ln -s /home/guest /etc/guest-session/skel```

```sudo nano /etc/lightdm/lightdm.conf```

```[SeatDefaults]
autologin-guest=true```

```sudo nano /etc/guest-session/prefs.sh
touch $HOME/.skip-guest-warning-dialog```