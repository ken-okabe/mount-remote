mount-remote
============


###1. install OSXFUSE 
http://sourceforge.net/projects/osxfuse/

osxfuse-{VERSION}.dmg 

check `Mac FUSE Compatibility Layer` while install

###2. Install SSHFS
https://github.com/osxfuse/sshfs/downloads

SSHFS-{VERSION}.pkg 

###3. Confirm 
$ sshfs --version

SSHFS version 2.4 (OSXFUSE SSHFS 2.4.1)

OSXFUSE library version: FUSE 2.7.3 / OSXFUSE 2.6.2

no mount point

###4. Mount
$ sshfs [user@]host:[dir] mountpoint [options]

mkdir remote

sshfs -o IdentityFile=/Volumes/GD15/gd1/azure/myPrivateKey.key ken@some-host.cloudapp.net:/ ~/remote
