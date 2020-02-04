
rofmus — Music Player
=====================

a simple fork of cmus — C\* Music Player
https://github.com/cmus/cmus

Changes from the original
---------------------
The ablum and playlist views are smaller.

Can be changed with the cmus command :resize-view <num>  
a larger number will make the playlist view larger.


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

To disable some feature, arts for example, and install to `$HOME` run

    $ ./configure prefix=$HOME CONFIG_ARTS=n

After running configure you can see from the generated `config.mk` file
what features have been configured in (see the `CONFIG_*` options).

Install To Temporary
--------------------

    $ make install DESTDIR=~/tmp/cmus

This is useful when creating binary packages.

Manuals
-------

    $ man cmus-tutorial
    $ man cmus

Reporting Bugs
--------------
*Warning: cmus is not actively maintained. For details, please see [#856](https://github.com/cmus/cmus/issues/856)*

Firstly search for any existing issues at cmus [issues](https://github.com/cmus/cmus/issues).
if you can't find your problem or bug then create one at rofmus [issues](https://github.com/roflcoffel/cmus/issues).

Additional debug information can be found in `~/cmus-debug.txt` if you configured cmus with
maximum debug level (`./configure DEBUG=2`). In case of a crash the last lines may be helpful.


