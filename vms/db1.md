---
layout: default
title: 'db1 - Database Server'
---
# db1 - Database Server #

db1 is the primary database server for NCMLS. In an effort to distribute the various components and enable later scaling as needed, database hosting was split into a separate VM. 

## Services ##

db1 runs 2 services:

* [MySQL](http://www.mysql.com/) is *the* standard for open-source SQL systems. This is db1's primary role / service.
* [phpMyAdmin](http://www.phpmyadmin.net/home_page/index.php) is a tool for managing a MySQL server. It provides a PHP-based web interface for administering privileges and databases within MySQL.

## Web Properties ##

Other than the web-based interface for phpMyAmdmin, none.

## Scheduled Tasks (cron) ##

db1 runs 1 scheduled task: every 6 hours (at 5:55AM/PM, 11:55AM/PM), a complete database export is run by the bmschell user account and placed in a folder within that user's home directory. This script does not do any rotating of backups, resulting in required maintenance every other month or so to manage (read: deleting) old backups. This script needs to be updated in the near future to remove old files and optionally move files to an offsite backup (Amazon S3?).