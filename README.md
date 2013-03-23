tmux 1.8 .debs for Debian Lenny 32bit
=====================================
(Packaged with `checkinstall`)

Installation
------------
- First make sure no tmux package from the debian repos is installed.
- `sudo dpkg -i libevent-2.0-5_2.0.16-stable-1_i386.deb`, followed by `sudo dpkg -i tmux_1.8-1_i386.deb`. OR place those 2 pacakges in a local apt-repo and install using apt-get.

Building
--------
- Install the `libevent-dev-2.0.16_stable-1-1_i386.deb` package
- Make the `checkinstall`, `automake`, and `libncurses5-dev` packages are installed.
- Follow the build instructions here: http://sourceforge.net/p/tmux/tmux-code/ci/master/tree/README, except substitute any `make install` with `sudo checkinstall -D`
