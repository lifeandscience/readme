---
layout: default
title: 'lb1 - Load Balancer'
---
# lb1 - Load Balancer #

The purpose of lb1 is to act as a frontend for all web-based requests related to MLS's web presence. This has several advantages, most notably that the only public-facing IP address that is openly published is the one for lb1; all other VMs aren't publicly advertised as being a part of MLS's infrastructure. Instead, all traffic goes through lb1 and then distributed to the other VMs via Linode's internal network.

## Services ##

lb1 runs 1 service: nginx. [nginx](http://nginx.org/) is a fast web server and proxy. It's configuration on lb1 is primarily as a reverse proxy, routing requests that come from the public-facing IP to web servers running on other VMS on the internal network.

## Web Properties ##

None.

## Scheduled Tasks (cron) ##

None.