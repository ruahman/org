+++
title      = "fdisk"
date       = 2026-10-11T19:20:11-04:00
tags       = ["cli", "terminal"]
identifier = "20261011T192011"
+++

# fdisk

`fdisk -l` : list disks in your device

`fdisk /path/to/disk` : enter fdisk prompt for disk

`m` : type m for help

`p` : print disk and partitions

`g` : create gpt partition table

`n` : new partition

`w` : write

`mkfs.ext4 /device/path` : formate disk

`lsblk` : list block devices

`umount /path/to/mount` : unmount disk

`mount` : show all mount points
mounting is attaching a storage device to the file system
you can mount where ever but the convention is in **/mnt** or **/media**
**/media** is for attached media like flash drives

`sudo mount /dev/sdb1 /mnt/disk1`

`/etc/fstab` : list divices that automaticaly get mounted

`fdisk` : is for setting up partitions

`mkfs`  : is for formating disks

`lsblk` : list block devices
