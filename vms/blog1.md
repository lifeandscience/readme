---
layout: default
title: 'blog1 - Blog Web Server'
---
# blog1 - Blog Web Server

blog1 is the blog web server for NCMLS, hosting a Multisite-enabled Wordpress install and a proof-of-concept of the www.ncmls.org redesign.

## Services ##

blog1 runs 1 service: [apache](http://projects.apache.org/projects/http_server.html). Apache is configured to host a vhost for each of the web properties outlined below.

## Web Properties ##

blog1 handles two web properties:

* All properties based on the [Multisite-enabled Wordpress installation](../sites/wordpress-blog.html).
* The proof-of-concept for the [new NCMLS website](../sites/new.html).

## Scheduled Tasks (cron) ##

None.