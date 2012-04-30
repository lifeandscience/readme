---
layout: default
title: 'em1 - Experimonth Web Server'
---
# em1 - Experimonth Web Server

em1 is the web server for Experimonth, hosting a Multisite-enabled Wordpress install and node.js-based properties related to Experimonth: Race.

## Services ##

em1 runs 3 services:

* [apache](http://projects.apache.org/projects/http_server.html). Apache is configured to host the vhost for the Wordpress and Vanilla Forums installs mentioned below
* A node.js-based server for Experimonth: Race (mentioned below)
* [MongoDB](http://www.mongodb.org/) - A NoSQL database system, used by the node.js-based Experimonth: Race app. Eventually, it'd be best to move this to db1 to better separate responsibilities.

## Web Properties ##

em1 handles three web properties:

* A Multisite-enabled Wordpress install which handles [experimonth.lifeandscience.org](../sites/wordpress-experimonth.html).
* An installation of [Vanilla Forums](../sites/vanilla-forums.html) , tracked by a [Git repository](https://github.com/lifeandscience/Garden)
* The node.js-based application for [Experimonth: Race](../sites/node-experimonth.html).

## Scheduled Tasks (cron) ##

None.