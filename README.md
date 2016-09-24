terminal, simple serial terminal in Python
====

This is a fork of Jim Paris' work at
https://git.jim.sh/jim/terminal.git. I've quoted his documentation in
`terminal.py` below:

Simple terminal program for serial devices.  Supports setting
baudrates and simple `LF->CRLF` mapping on input, and basic flow
control, but nothing fancy.

^C quits.  There is no escaping, so you can't currently send this
character to the remote host.  Piping input or output should work.

Supports multiple serial devices simultaneously.  When using more than
one, each device's output is in a different color.  Input is directed
to the first device, or can be sent to all devices with --all.
