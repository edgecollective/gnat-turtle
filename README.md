# gnat-turtle
gnat-based turtle tracker

## PI

### formatting microsd in linux

https://ragnyll.gitlab.io/2018/05/22/format-a-sd-card-to-fat-32linux.html

### copying microSD in linux

sudo dd if=/dev/mmcblk0 of=./rak-chirp-03-08-20-pi-01.img status=progressA

### removing and generating new ssh host keys

```
sudo rm /etc/ssh/ssh_host*
sudo ssh-keygen -A
```

