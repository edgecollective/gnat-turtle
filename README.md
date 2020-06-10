# gnat-turtle
gnat-based turtle tracker

## PI

### formatting microsd 

- In [Linux](https://ragnyll.gitlab.io/2018/05/22/format-a-sd-card-to-fat-32linux.html)

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

NOTE: this shows progress, but doesn't produce a viable zip file:

```pv rak-chirp-03-08-20-pi-01.img | zip > rak1.zip
```

Instead, use:

```
zip rak2.zip rak-chirp-team-1602885022-date-2020-06-08.img 
```

