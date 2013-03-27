dd if=/dev/zero bs=1024k count=2048 >> 2013-02-09-wheezy-raspbian.img

fdisk 2013-02-09-wheezy-raspbian.img
Command (m for help): m
Command action
   a   toggle a bootable flag
   b   edit bsd disklabel
   c   toggle the dos compatibility flag
   d   delete a partition
   l   list known partition types
   m   print this menu
   n   add a new partition
   o   create a new empty DOS partition table
   p   print the partition table
   q   quit without saving changes
   s   create a new empty Sun disklabel
   t   change a partition's system id
   u   change display/entry units
   v   verify the partition table
   w   write table to disk and exit
   x   extra functionality (experts only)

Command (m for help): p

Disk 2013-02-09-wheezy-raspbian.img: 4087 MB, 4087349248 bytes
255 heads, 63 sectors/track, 496 cylinders, total 7983104 sectors
Units = sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disk identifier: 0x00014d34

                         Device Boot      Start         End      Blocks   Id  System
2013-02-09-wheezy-raspbian.img1            8192      122879       57344    c  W95 FAT32 (LBA)
2013-02-09-wheezy-raspbian.img2          122880     3788799     1832960   83  Linux

Command (m for help): d
Partition number (1-4): 2

Command (m for help): n
Partition type:
   p   primary (1 primary, 0 extended, 3 free)
   e   extended
Select (default p): p
Partition number (1-4, default 2): 2
First sector (2048-7983103, default 2048): 122880
Last sector, +sectors or +size{K,M,G} (122880-7983103, default 7983103):
Using default value 7983103

Command (m for help): w
The partition table has been altered!

Syncing disks.

