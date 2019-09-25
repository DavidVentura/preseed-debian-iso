# preseed-debian-iso
Preseeds a debian iso

Tested so far with 

* debian-9.9.0-amd64-netinst.iso
* debian-10.1.0-amd64-netinst.iso

It should work for most debian based ISOs.


If you plan to use this, configure your preseed.cfg for your usecases.  
Keep in mind that you *have* to change:

* mirror/http/proxy
* passwd/root-password-crypted (default password is 'on')
* time/zone
* partman-auto/disk (depending on your qemu setup; for VirtIO I get a /dev/vda
  disk)
* partman-auto/expert\_recipe (for disk layout)


## Demo

[![asciicast](https://asciinema.org/a/254415.svg)](https://asciinema.org/a/254415)
