My personal kernel and buildroot configs for retroleap

Kernel Config: lf2000-kernel-config

Buildroot Config: lf2000-buildroot-config (configured for this buildroot environment https://github.com/mac2612/retroleap.git)
As this buildroot config uses gcc12, the kernel has to be built seperate (the retroleap kernels can only be buuilt with gcc 4)
If you use my kernel config the required modules for the usb ethernet are built in, otherwise you have to build just the kernel first (make linux)
then do the rootfs using this buildroot config (make rootfs-tar)

LF2000-OC-Patch = the patch files used for the kernel. Normal users wont need this. The OC kernel on my github (https://github.com/DCFUKSURMOM/lf2000_kernel-oc.git)
already has this applied, this is just a backup.

The patch was provided by mac2612 (https://github.com/mac2612) but its not on their GitHub (yet). In the future I
want to add a slightly less overclocked patch for devices that dont like the 800mHz, I'll have to talk to mac2612 or andymcca about getting it working as its
out of my skill level.

Realtime patch = kinda self explanitory, realtime patch file for my kernel
