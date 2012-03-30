---
layout: default
title: 'monitor - Monitoring + DNS'
---
# monitor - Monitoring + DNS #

The purpose of monitor is to act as a always-on monitoring VM, an internal DNS service (for resolving these hostnames which aren't published externally), and a space for experimenting with other monitoring or analytics services. Presently it's monitoring role is a bit superfluous; while it has Munin and other monitoring systems installed, they aren't used with any regularity. The most important service, by far, is the DNS server.

Eventually, monitor or [lb1](lb1.html) could be used for scheduled utility jobs (via Cron); however presently those happen on whatever machine the service or application is installed on.

## Services ##

monitor runs 3 services:

* [Munin](http://munin-monitoring.org/) is a system monitoring service; it connects to configured nodes to collect data on their status. Munin can be accessed via [http://monitor.lifeandscience.org/munin](http://monitor.lifeandscience.org/munin).
* [Zabbix](http://www.zabbix.com/) is "an enterprise-class open source distributed monitoring solution for networks and applications." (from their site). It was installed in July 2011 during the infrastructure setup but is sufficiently complex (read: overkill) for the MLS infrastructure. It's configuration has not gone beyond basic setup and it should probably be removed. [http://monitor.lifeandscience.org/zabbix](http://monitor.lifeandscience.org/zabbix).
* [Unbound](http://unbound.net/) is "a validating, recursive, and caching DNS resolver". It's used to provide a local DNS server to the MLS VMs; each is configured to use monitor.lifeandscience.org as it's DNS server. Static entries are configured within unbound to resolve the internal hostnames (e.g. db1.lifeandscience.org).

## Web Properties ##

Other than the web-based interfaces to Munin (and Zabbix), none.

## Scheduled Tasks (cron) ##

None.