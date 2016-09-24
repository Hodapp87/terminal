terminal, simple serial terminal in Python
====

This is a fork of Jim Paris' work at
https://git.jim.sh/jim/terminal.git. I fixed a bug that kept it from
running on Python 3.x, added a feature to log to a file, and emailed
Jim a patch in October 2015 - however, I never heard back from him, so
my changes are here.

I've quoted his documentation in `terminal.py` in the section below.

Documentation
----

Simple terminal program for serial devices.  Supports setting
baudrates and simple `LF->CRLF` mapping on input, and basic flow
control, but nothing fancy.

^C quits.  There is no escaping, so you can't currently send this
character to the remote host.  Piping input or output should work.

Supports multiple serial devices simultaneously.  When using more than
one, each device's output is in a different color.  Input is directed
to the first device, or can be sent to all devices with --all.
