# Leapdroid-virtual-device
This project  contains source code for a VirtualBox virtual device. The virtual device is a channel by which the Android vm and the host communicate. 

More info can be found on our website at http://www.leapdroid.com

In order for the android vm to talk to the host machine, a linux kernel module must be present inside the vm. On the host side, vbox will add a virtual device. The kernel module and the virtual device communicate with each other through standard hardware i/o emulations provided by vbox. This is the fundenmatal pieces for any vm guest additions. We use these mechanims for vm to forward opengl calls, for host to send inputs, etc.

