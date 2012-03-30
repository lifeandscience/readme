---
layout: default
title: 'Experimonth Wordpress - Handling Experimonth-related blogs / applications'
---
# Experimonth Wordpress - Handling Experimonth-related blogs / applications

Experimonth Wordpress is a [Wordpress](http://wordpress.org)-powered blog network. It is setup using Wordpress configured with Multisite enabled, allowing it to host multiple subfolder-based blogs. 

This Wordpress instance also has an installation of [Mint](http://haveamint.com/) running alongside it. It's automatically tracked on every PHP-based request using auto_prepend_file in the .htaccess file.

## Sites ##

* [experimonth.lifeandscience.org](http://experimonth.lifeandscience.org) - the top-level landing page and 'primary' blog.
* [experimonth.lifeandscience.org/mood](http://experimonth.lifeandscience.org/mood) - the blog (and plugin functionality) for Experimonth: Mood.

## Server ##

The Wordpress instance is hosted on [em1](../vms/em1.html).

## Database ##

This Wordpress instance uses the 'experimonth' MySQL database hosted by [db1](../vms/db1.html). The Mint install uses the 'mint_experimonth' MySQL database hosted by [db1](../vms/db1.html).