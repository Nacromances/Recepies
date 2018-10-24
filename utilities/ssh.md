# ssh tips and tricks

## Mount remote file system on sshfs

* create a mount dir 
`sudo mkdir /mnt/mysys`
* mount using sshfs
`sudo sshfs -o allow_other,defer_premission xxx@yyy`


