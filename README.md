# core-riscv64 ports

## Rootfs (2024-09-22) from core and opt ports is now available on

https://sourceforge.net/projects/rootfs-riscv64/files/


### MACHINE (model V1.3b)
\# cat /sys/firmware/devicetree/base/model

\# StarFive VisionFive V2

### CPU

\# cat /proc/cpuinfo

processor       : 0

hart            : 1

isa             : rv64imafdc

mmu             : sv39

isa-ext         :

uarch           : sifive,u74-mc

processor       : 1

hart            : 2

isa             : rv64imafdc

mmu             : sv39

isa-ext         :

uarch           : sifive,u74-mc

processor       : 2

hart            : 3

isa             : rv64imafdc

mmu             : sv39

isa-ext         :

uarch           : sifive,u74-mc

processor       : 3

hart            : 4

isa             : rv64imafdc

mmu             : sv39

isa-ext         :

uarch           : sifive,u74-mc

### MEMORY
\# free -h

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;used&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;free&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;shared&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;buff/cache&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;available

Mem:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7.7Gi&nbsp;&nbsp;&nbsp;177Mi&nbsp;&nbsp;&nbsp;7.6Gi&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;488Ki&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;85Mi&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7.6Gi

Swap:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8.0Gi&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0B&nbsp;&nbsp;&nbsp;&nbsp;8.0Gi

### STORAGE
\# df -Th

Filesystem     Type      Size  Used Avail Use% Mounted on

/dev/root      ext4       59G  3.4G   53G   6% /

devtmpfs       devtmpfs  3.6G     0  3.6G   0% /dev

run            tmpfs     3.9G  488K  3.9G   1% /run

shm            tmpfs     3.9G     0  3.9G   0% /dev/shm

cgroup         tmpfs     3.9G     0  3.9G   0% /sys/fs/cgroup

/dev/mmcblk1p3 vfat      292M   30M  263M  10% /boot

/dev/nvme0n1p5 ext4       98G  5.5G   88G   6% /home

pkgbuild       tmpfs     8.0G     0  8.0G   0% /home/devel/building

\# lspci

0000:00:00.0 PCI bridge: PLDA XpressRich-AXI Ref Design (rev 02)

0000:01:00.0 USB controller: VIA Technologies, Inc. VL805/806 xHCI USB 3.0 Controller (rev 01)

0001:00:00.0 PCI bridge: PLDA XpressRich-AXI Ref Design (rev 02)

0001:01:00.0 Non-Volatile memory controller: MAXIO Technology (Hangzhou) Ltd. NVMe SSD Controller MAP1202 (rev 01)
