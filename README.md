# Icecast 2.3.2

Icecast is a streaming media server which currently supports Ogg
streaming including the vorbis and theora codecs. Also icecast can
handle other streams like MP3/AAC/NSV.
It can be used to create an Internet radio station or a privately
running jukebox and many things in between. It is very versatile in
that new formats can be added relatively easily and supports open
standards for communication and interaction.

This version was based off of the 2.3.2 trunk, and includes extra
functionality added by Nicholas Young (of Original Machine). Extra
documentation on these additions is forthcoming.

Icecast is distributed under the GNU GPL, version 2. A copy of this
license is included with this software in the COPYING file.

## Prerequisites

Icecast requires the following packages:

* libxml2 - http://xmlsoft.org/downloads.html
* libxslt - http://xmlsoft.org/XSLT/downloads.html
* curl - http://curl.haxx.se/download.html (>= version 7.10 required)
* ogg/vorbis - http://www.vorbis.com/files (>= version 1.0 required)

#### NOTE:

Icecast may be compiled without curl, however this will disable Stream Directory server interaction (YP) and URL based authentication.

### A note about prerequisite packages

Most distributions have some sort of package management repository for
pre-built packages (eg rpm, deb etc).  These setups often have a runtime
package, which is usually installed for you by default, and enables you
to run applications that depend on them.  However if you are building
icecast from source then the runtime system is not enough. You will also
need a development package named something like libxslt-devel

## Build/Install

To build icecast on a Unix platform, perform the following :

Run
* ./configure
* make
* make install

This is the typical procedure if you download the tar file.  If you retrive
the code from subversion or want to rebuild the configure then run autogen.sh
instead of the configure above. Most people do not need to run autogen.sh

A sample config file will be placed in /usr/local/etc (on UNIX) or in 
the current working directory (on Win32) and is called icecast.xml

Documentation for icecast is available in the doc directory, by 
viewing doc/index.html in a browser.

Please email us at icecast@xiph.org or icecast-dev@xiph.org, or come and see
us at irc.freenode.net, channel #icecast, if you have any troubles.