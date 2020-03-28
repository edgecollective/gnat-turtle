# gnat-turtle
gnat-based turtle tracker

## PI

### formatting microsd 

- In [Linux](https://ragnyll.gitlab.io/2018/05/22/format-a-sd-card-to-fat-32linux.html)

to figure out which disk:

```
sudo fdisk -l
```

e.g. mmcblk0

unmount the disk

then to erase partitions, run the command:

```
sudo fdisk /dev/mmcblk0
```

then use:

```
p
n
(accept defaults)
t
b
w
```

then to format:

```
mkfs.vfat /dev/mmcblk0p1
```





### copying microSD in linux

```
sudo dd if=/dev/mmcblk0 of=./rak-chirp-03-08-20-pi-01.img status=progress
```

### removing and generating new ssh host keys

```
sudo rm /etc/ssh/ssh_host*
sudo ssh-keygen -A
```

### zipping and showing progress

pv rak-chirp-03-08-20-pi-01.img | zip > rak1.zip

