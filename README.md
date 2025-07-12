# QEMU X86 Artifacts

**Required Components:**
All necessary artifacts for running QEMU with X86 processor emulation.

## Command Execution
To launch the QEMU X86 emulator, use the following configuration:

```bash
qemu-system-x86_64 \
    -kernel bzImage \
    -serial stdio \
    -append "console=ttyS0 nokaslr root=/dev/ram rdinit=/linuxrc noacpi" \
    -initrd rootfs.img.gz \
    -m 512


To launch the QEMU X86 emulator with 4 cores, use the following configuration:

```bash
qemu-system-x86_64 \
    -kernel bzImage \
    - smp 4  \
    -serial stdio \
    -append "console=ttyS0 nokaslr root=/dev/ram rdinit=/linuxrc noacpi" \
    -initrd rootfs.img.gz \
    -m 512

