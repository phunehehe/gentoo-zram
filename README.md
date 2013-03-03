Init script for zRam, intended for Gentoo, tested on Funtoo (OpenRC)

For more information on setting up zRam on Gentoo, see
http://wiki.gentoo.org/wiki/Zram. This init script is a replacement for [Martin
Väth's](https://github.com/vaeth/zram-init), which requires configurations in
`/etc/conf.d/zram-init`.

This init script automatically determines the size of zRam based on the amount
of RAM the sytem has. The size of zRam is equal to the amount of RAM. Note that
this size is uncompressed, which means the actual size that zRam uses in memory
will be smaller, around a third of RAM.


The code is adapted from the package [`zram-config` in
Ubuntu](https://launchpad.net/ubuntu/+archive/primary/+files/zram-config_0.1.tar.gz).


Copyright © 2013 Hoàng Xuân Phú

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program. If not, see http://www.gnu.org/licenses/.
