 # crux-ports-cubieboard2-arm

CRUX-ARM ports overlay for Cubieboard 2

To use these ports, download the `cubieboard2-arm.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/crux-arm/crux-ports-cubieboard2-arm/3.7/cubieboard2-arm.httpup
$ sudo ports -u cubieboard2-arm
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/cubieboard2-arm
prtdir /usr/ports/core-arm
prtdir /usr/ports/opt-arm
prtdir /usr/ports/xorg-arm
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
