
rofmus — Music Player
=====================

a simple fork of cmus — C\* Music Player
https://github.com/cmus/cmus

Install from source
-------------------
Clone this project with

    $ git clone https://github.com/roflcoffel/cmus.git

Auto-detect configuration

    $ ./configure

Build the project

    $ make

Install

    $ make install


Detailed Configuration
----------------------
List available optional features

    $ ./configure --help

Auto-detect everything

    $ ./configure

To disable some feature, arts for example, and install to `$HOME` run

    $ ./configure prefix=$HOME CONFIG_ARTS=n

After running configure you can see from the generated `config.mk` file
what features have been configured in (see the `CONFIG_*` options).

*Note*: For some distributions you need to install development versions
of the dependencies.  For example if you want to use 'mad' input plugin
(mp3) you need to install `libmad0-dev` (Debian) or `libmad-devel` (RPM)
package. After installing dependencies you need to run `./configure`
again, of course.

If you want to use the Tremor library as alternative for decoding
Ogg/Vorbis files you have to pass `CONFIG_TREMOR=y` to the configure
script:

    $ ./configure CONFIG_VORBIS=y CONFIG_TREMOR=y

The Tremor library is supposed to be used on hardware that has no FPU.


Building
--------

    $ make


Installation
------------

    $ make install

Or to install to a temporary directory:

    $ make install DESTDIR=~/tmp/cmus

This is useful when creating binary packages.

Manuals
-------

    $ man cmus-tutorial

And

    $ man cmus


Reporting Bugs
--------------
*Warning: cmus is not actively maintained. For details, please see [#856](https://github.com/cmus/cmus/issues/856)*

Firstly search for any existing issues at cmus [issues](https://github.com/cmus/cmus/issues).
if you can't find your problem or bug then create one at rofmus [issues](https://github.com/roflcoffel/cmus/issues).

Additional debug information can be found in `~/cmus-debug.txt` if you configured cmus with
maximum debug level (`./configure DEBUG=2`). In case of a crash the last lines may be helpful.


