# About

ptouch is a command line tool to print labels on Brother P-Touch
printers on Linux.

There is no need to install the printer via CUPS, the printer is accessed
directly via libusb.

The tool was written for and tested with the PT-2430PC, but it should also
work with the PT-1230PC (untested so far).
Maybe others work too (please report USB VID and PID so I can include support
for further models, too).

To build on Ubuntu:

```
sudo apt-get -y install libusb-1.0-0-dev autopoint autoconf libgd-dev
autoreconf -i
./configure --prefix=/usr
make -j$(nproc)
sudo make install
```

Further info can be found at:
https://mockmoon-cybernetics.ch/computer/p-touch2430pc/
