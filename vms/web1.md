---
layout: default
title: 'web1 - Primary Web Server'
---
# web1 - Primary Web Server

web1 is the primary web server for NCMLS, hosting a number of web properties as outlined below. 

## Services ##

web1 runs 1 service: [apache](http://projects.apache.org/projects/http_server.html). Apache is configured to host a vhost for each of the web properties outlined below.

## Web Properties ##

web1 handles several web properties:

* All properties based on the [Drupal 5 installation](../sites/drupal.html)
* [Lessn More](https://github.com/alanhogan/lessnmore), a [URL Shortener](../sites/lessn.html)
* The [ThinkUp](http://thinkupapp.com/) [installation](../sites/thinkup.html)
* Several smaller static directories:
	* [summercamp.lifeandscience.org](../sites/summercamp.html)
	* [www.ncmls.org/collecting](../sites/collecting.html)
	* [www.ncmls.org/{beck,kelly}](../sites/beck_n_kelly.html)

## Scheduled Tasks (cron) ##

web1 runs 1 schedule task: once hourly, the ThinkUp updater script is run to crawl the configured social accounts. This happens locally using the command-line PHP, so it must run local on this VM.