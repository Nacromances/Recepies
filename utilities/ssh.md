# ssh tips and tricks

## Mount remote file system on sshfs

* create a mount dir 
`sudo mkdir /mnt/mysys`
* mount using sshfs
`sudo sshfs -o allow_other,IdentityFile=<PathToIdentityFile> xxx@yyy:zzz /mnt/mysys`
where
** PathToIdentityFile is the private key used to log to remove xxx@yyy
** xxx is the username on yyy
** yyy is the host of the remote filesystem directory
** zzz is the directory we want to mount
** /mnt/mysys is mounting point.




