---
title: Setting up my Cloud Security Lab on GCP, Azure and AWS.
date: 2026-02-13 10:07:00 +0300
categories: [Cloud, Lab-Setup, Azure, AWS, GCP]
tags: [ubuntu, nginx, gcp,aws, azure]
image:
  path: assets/aws-azure-gcp.jpg
  alt: A feature image for awsazuregcp

---
## Why I built this Lab
To truly understand **Network Security**, I decided to move away from local VMs and deploy a dedicated environment on **GCP**

### The Architecture
I am currently running on **Ubuntu 22.04** instance named *Lab1*. My goals for this setup include:
1: Configuring hardened *Nginx* Reverse Proxy.
2: Managing Access via *Custom SSH Ports* top reduce bruteforce noise.
3:Hosting my technical documentation(this blog!) via GitHub Pages

### Lessons Learnt
During this setup I encountered isssues with **Bitlocker** encrypted drives on my local machine

---
*Stay tuned for my next post*
