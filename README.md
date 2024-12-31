# EXT2-Filesystem
# Hey! I'm Filing Here

In this lab, I successfully implemented 1 MiB ext2 file system with 2 directories, 1 regular file, and 1 symbolic link.

## Building
You can make the executable ext2-create by running 
```
make
```


## Running
Run ./ext2-create to create cs111-base.img
Run fsck.ext2 cs111-base.img to check the errors of the file system.
Run dumpe2fs cs111 -base.img which dumps filesystem information and is helpful for debugging.
Run mkdir mnt, which is the directory you mount the filesystem too.
```
./ ext2 - create # run the executable to create cs111 -base.img
dumpe2fs cs111 -base.img # dumps the filesystem information to help debug
fsck.ext2 cs111 -base.img # this will check that your filesystem is correct
mkdir mnt # create a directory to mnt your filesystem to
sudo mount -o loop cs111 -base.img mnt # mount your filesystem , loop lets you use a file
sudo umount mnt # unmount the filesystem when you 're done
rmdir mnt # delete the directory used for mounting when you 're done
```


## Cleaning up

```
make clean
```

If you wish to unmount the filesystem you can run, 
```
sudo umount mnt # unmount the filesystem when you 're done
rmdir mnt # delete the directory used for mounting when you 're done
```
