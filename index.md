---
title: set-dns
layout: default
---
set-dns
=======

A simple shell script to set DNS servers on MacOS X 10.5+ using scutil(1). 

[http://dossy.github.com/set-dns](http://dossy.github.com/set-dns)

Copyright (c) 2010, Dossy Shiobara &lt;dossy@panoptic.com&gt;

DESCRIPTION
-----------

set-dns is a simple shell script to simplify the changing of the
PrimaryService's DNS server list under MacOS X 10.5+ using the
scutil(1) utility.

DOWNLOAD
--------

The script is hosted in a Git repository at GitHub.com:

[http://github.com/dossy/set-dns](http://github.com/dossy/set-dns)

INSTALLATION
------------

Copy set-dns.conf to /etc/defaults, and set-dns to /usr/bin:

    $ sudo cp set-dns.conf /etc/defaults
    $ sudo cp set-dns /usr/bin
    $ sudo chmod 0755 /usr/bin/set-dns

Edit /etc/defaults/set-dns.conf with the default servers you wish to
use.  This should be one or more IP addresses separated with spaces.
By default, SERVERS is set to "192.168.1.1".

USAGE
-----

    Usage: set-dns [OPTION]... [SERVER]...
    Show or set the DNS servers for the PrimaryService using scutil(1).

      -c <file>  use <file> as the config file, instead of
                   /etc/defaults/set-dns.conf
      -s         set server list
      -?         display this help and exit

LICENSE
-------

This script and associated files are hereby licensed under a
simplified BSD-style license.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:

        1. Redistributions of source code must retain the above
           copyright notice, this list of conditions and the following
           disclaimer.
        2. Redistributions in binary form must reproduce the above
           copyright notice, this list of conditions and the following
           disclaimer in the documentation and/or other materials
           provided with the distribution.

    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
    "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
    LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
    FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
    COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
    INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
    BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
    LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
    ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
    POSSIBILITY OF SUCH DAMAGE.
