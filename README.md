Ralink Driver
=============
This is an attempt to bring ralink back to life. Previous instructions were available [here](http://bernaerts.dyndns.org/linux/74-ubuntu/229-ubuntu-precise-dlink-dwa160-revb2).

Usage
-----
These instructions have been tested on Ubuntu 14.04.

1. Remove USB card, then remove existing kernel modules:

        sudo rmmod rt2800usb
        sudo rmmod rt2x00usb
        sudo rmmod rt2800lib
        sudo rmmod rt2x00lib

2. Get pre-requisits:

        sudo apt-get install build-essential

3. Download source code

        git clone https://github.com/cristiklein/ralink.git

4. Compile source code

        cd ralink
        make

5. Install module

        sudo make install

6. Load module

        sudo modprobe rt5572sta

Tested with
-----------
* 2001:3c1a D-Link Corp. DWA-160 802.11abgn Xtreme N Dual Band Adapter(rev.B2) [Ralink RT5572]

Contact
-------
Please contact <cristiklein@gmail.com> for feedback.

