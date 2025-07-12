# qemu_x86_artifact1
All artifact required for Qemu X86 processor

#to run using following command
qemu-system-x86_64 -kernel bzImage -serial stdio -append "console=ttyS0 nokaslr root=/dev/ram rdinit=/linuxrc noacpi"  -initrd rootfs.img.gz -m 512
