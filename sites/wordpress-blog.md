---
layout: default
title: 'Blog Wordpress - Handling blogs.ncmls.org'
---
# Blog Wordpress - Handling blogs.ncmls.org

Blog Wordpress is a [Wordpress](http://wordpress.org)-powered blog network. It is setup using Wordpress configured with Multisite enabled, allowing it to host multiple subfolder-based blogs. 

## Sites ##

* [blogs.ncmls.org](http://blogs.ncmls.org) - the top-level landing page and 'primary' blog. It's actually not accessible publicly as blogs.ncmls.org is redirected to a page on the [Drupal-powered main site](drupal.html).
* [blogs.ncmls.org/keepers](http://blogs.ncmls.org/keepers) - the Animal Keepers blog
* [blogs.ncmls.org/greg-dodge](http://blogs.ncmls.org/greg-dodge) - Greg Dodge Journal
* [blogs.ncmls.org/crashtest](http://blogs.ncmls.org/crashtest) - Crash Test blog setup for an exhibit; never publicized (?)

## Server ##

The Wordpress instance is hosted on [blog1](../vms/blog1.html).

## Database ##

This Wordpress instance uses the 'wpmu' MySQL database hosted by [db1](../vms/db1.html).