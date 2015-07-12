[![Stories in Ready](https://badge.waffle.io/proidiot/hextime-bash.png?label=ready&title=Ready)](https://waffle.io/proidiot/hextime-bash)
# hextime-bash
hextime is a hexadecimal representation of the actual number of seconds which
have passed since the Unix epoch (exactly midnight of 1 January 1970 UTC).
Unlike some other measures of time, hextime does not include leap seconds;
hextime is intended to be a linear measure of real time.

hextime-bash is an implementation of hextime in the bash scripting language.

Note
----
This version ships with a copy of the IETF list of leap second offsets, but it
will currently prompt the user to redownload [the list from the IETF website](http://www.ietf.org/timezones/data/leap-seconds.list) if
the list is a year old. At some point, I'd rather change the URL to a dedicated
mirror.

License
-------
hextime-bash Copyright (C) 2015  Charles Southerland

This program is released under the terms of the GNU GPL v3 or later.
This program comes with ABSOLUTELY NO WARRANTY.
This is free software, and you are welcome to redistribute it under certain
conditions.See [the GNU licenses site](https://www.gnu.org/licenses/) for details.

Bugs
----
Please report bugs through [github](https://github.com/proidiot/hextime-bash/issues).

