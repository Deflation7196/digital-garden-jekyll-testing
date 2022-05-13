---
title: 
---
links [[the-wire]] [[Why planning matters]]
# My Current Home Lab Setup
I currently have a modest Home Lab much like cars you can never have enough gadgets and parts. If you're of the more paranoid mindset you may also keep your hardware within the vendor life cycle which can get pricey very quick. I use my home lab more as a sandcastle and less as a constant hosting infrastructure although that tends to change with my mood. Currently I have four Raspberry PI's two of them are PI 4 8GB models that power my k3s cluster, one is a PI 3B+ that controls my pi-hole, and the last one is a PI 2 that runs octoprint connected to my [[CR10 3D Printer]] via USB interfacing over serial. Along with all of that I have a TrueNAS server that's powered by a Think-Station.

#### Raspberry PI's
The two Pi 4's are running k3s if I had a server rack and a better storage situation for the hardware I'd prefer to have k8s on larger super micro motherboards. I mostly run Google Alternatives in my kub cluster and connect in offsite via [ZeroTier](https://www.zerotier.com/). With more free time I would like to expand what I'm doing with kuberneties and expand the nodes in my cluster. 

The Pi 3 is running [DietPi](https://dietpi.com/) which is necessary with the hardware limitations and lack of fan on the current enclosure (something I need to fix). I currently run PI-Hole in a [[docker]] container I have a few other docker containers for hardening anything else would leave the Pi with little overhead to function

The final Pi is an older Pi 2 which controls my [[CR10 3D Printer]] with Octoprint, I have the Pi 2 hooked up to a ubiquity dish that's synced to a radio in my room I then give the Pi a static IP connecting it to my LAN wireless. This Pi sees some downtime as I'm not always 3d printing.

#### TrueNas
Just a generic Think-Station with ECC ram running TrueNAS off of a small SSD the drive capacity consist of four shucked 14TB WD drives, I'd enjoy more storage but currently power and space are limiting factors. In the future I'd like to mess around with Ceph and other software defined storage solutions.




