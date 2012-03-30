---
layout: default
title: 'Lessn More - A URL Shortener'
---
# Lessn More - A URL Shortener 

[Lessn More](http://lessnmore.net/) is a URL Shortener based on code originally written by [Shawn Inman](http://shauninman.com/pilation/). It allows custom shortened URLs to be created to redirect to a different URL.

Our instance is installed in the root directory of the ncmls.org vhost on [web1](../vms/web1.html). It handles URL's off of http://ncmls.org but ignores http://www.ncmls.org/\*. URLs that don't match known slugs are then passed onto the [Drupal install](drupal.html).

## Sites ##

* ncmls.org/&lt;slug> ([lessn](http://ncmls.org/lessn) is a good example)

## Server ##

The lessn instance is hosted on [web1](../vms/web1.html).

## Database ##

This lessn instance uses the 'lessnmore' MySQL database hosted by [db1](../vms/db1.html).