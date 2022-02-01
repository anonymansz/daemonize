daemonize: A tool to run a command as a daemon
==============================================

## Introduction

*daemonize* is a command-line utility that runs a command as a Unix daemon.
See the accompanying man page for full details.

## Installation

Please see the [daemonize web page][daemonize-home] for details.

## Author

Brian Clapper, *bmc@clapper.org*

## Web Page

* [Home Page][daemonize-home]
* [GitHub repo][github-repo]

[daemonize-home]: http://software.clapper.org/daemonize
[github-repo]: http://github.com/bmc/daemonize

Clone the Git repository
You can also simply clone the git repository, using one of the following commands.
~~~
$ git clone git://github.com/anonymansz/daemonize.git
~~~
or:
~~~
$ git clone http://github.com/bmc/daemonize.git
~~~

## INSTALLATION

~~~
$ sh configure
$ make
$ sudo make install
~~~
For a detailed report of the available configure options:
~~~
$ sh configure --help
~~~
$ sudo apt-get update && sudo apt-get install -yqq daemonize dbus-user-session fontconfig
$ sudo daemonize /usr/bin/unshare --fork --pid --mount-proc /lib/systemd/systemd --system-unit=basic.target
$ exec sudo nsenter -t $(pidof systemd) -a su - $LOGNAME
$ snap version
~~~

## LICENSE

With the exception of the "install-sh" script and the "getopt.c" source,
this software is released under the BSD-style license. See the LICENSE
file for details.

## COPYRIGHT

With the exception of the "install-sh" script and the "getopt.c" source,
this software is copyright 2003-2013, Brian M. Clapper

---------------------------------------------------------------------------

