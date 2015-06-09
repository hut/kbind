kbind
=====

kbind is a command-line tool to execute commands quickly with a single
keystroke.


Usage
-----

`kbind [statuscommand] <key>=<action>...`


Example
-------

`kbind ifconfig u='ifconfig eth0 up' d='ifconfig eth0 down'`

This will call *ifconfig* in each iteration, as a command that displays the
current status.

Whenever you type u into the console, the command `ifconfig eth0 up` will be
executed.  Conversely, typing d will execute `ifconfig eth0 down`.

Implicit key bindings are q for quitting the program and <SPACE> for rerunning
the status command.
