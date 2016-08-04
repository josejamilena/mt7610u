<u>**MT7610U for Linux**</u>

Driver for 802.11ac USB Adapter with MT7610U chipset  
Only STA Mode is supported, no AP.  

Monitor mode is not tested.

Currently tested on X86_64 platform(s) **only**,  
cross compile possible, but not fully tested.  

For compiling type  
`make`  
in source dir  

For install the driver use  
`sudo insmod mt7610u.ko`  

To Unload driver you need to disconnect the device

If the driver fails building consult your distro how to  
install the kernel sources and build an external module.
  
Questions about this will **silently** ignored !  
They are <u>plenty</u> information around the web.  

**BUGS**  
- can't unload driver, must disconnect device(s) first  
- can't compile on v4.7 or greater kernels  
  

**TODO**, in order of no appearance ;-)  
- fix unloading driver  
- update for v4.7 kernels cfg80211/nl80211 changes  
- do more function typesafe  
- cross compile check with real hw on $target  
- strip fw files and use kernel firmware load  
- check for wrong typecasts  
- remove/strip hardcoded `RT2870STA.dat`  
- check for wrong variable sizes (driver was for 32bit)  
- update to more USB-IDs  
- check if monitor mode is working  
- more cleanup and other stuff  
- fix compile warnings  
- misc. other stuff  


Hans Ulli Kroll <ulli.kroll@googlemail.com>




