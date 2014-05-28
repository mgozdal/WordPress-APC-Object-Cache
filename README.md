# WordPress APC Object Cache Backend #

Contributors: l3rady<br/>
Donate link: [http://l3rady.com/donate][2]<br/>
Tags: APC, object cache, backend, cache, performance, speed<br/>
Requires at least: 3.3<br/>
Tested up to: 3.9.1<br/>
Stable tag: ???

WordPress APC Object Cache Backend provides a persistent memory-based backend for the WordPress object cache.

## Description ##

WordPress APC Object Cache Backend provides a persistent memory-based backend for the WordPress object cache.

An object cache is a place for WordPress and WordPress extensions to store the results of complex operations. On subsequent loads,
this data can be fetched from the cache, which will be must faster than dynamically generating it on every page load.

Be sure to read the installation instructions, as this is **not** a traditional plugin, and needs to be installed in a specific location.

This object cache is a fork of [Mark Jaquith's APC Object Cache Backend][1]. There are a number of bugs in that version that have been
ignored so I decided to write my own version. The object cache has been pretty much been re-written but some of the best bits from Marks
version has been cherry picked over to this version.

## Installation ##

1. Verify that you have PHP 5.2.4+ and a compatible APC version installed.
2. Copy `object-cache.php` to your WordPress content directory (`wp-content/` by default).
3. Done!

## Frequently Asked Questions ##

### Does this support versions of WordPress earlier than 3.3? ###

Maybe, but I'm not going to support them, and you shouldn't still be running them!

### I share `wp-config.php` among multiple WordPress installs. How can I guarantee key uniqueness? ###

Define `WP_APC_KEY_SALT` to something that is unique for each install (like an md5 of the MySQL host, database, and table prefix).

## Changelog ##

### ??? ###
+ Initial release

[1]: https://wordpress.org/plugins/apc/
[2]: http://l3rady.com/donate