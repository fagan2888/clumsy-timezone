clumsy-timezone
===============

Javascript library to get a TZ timezone name (e.g. 'Asia/Bangkok') from an offset specified in minutes +/- (e.g. 420).

Made in Javascript for NodeJS.

It's called clumsy-timezone because:
* You can't reliably guess a timezone name from an offset. The timezone names used in the library are pretty arbitrary.
* No support for daylight savings.

Useful for:
* If you have only an offset but need a timezone name to use with other built-in functions.

Usage
======
clumsy = require('./clumsy-timezone.js')
tzname = clumsy.getTimezoneName(-360)
-> "America/Swift_Current"
process.env.TZ = tzname // hack-tastic
