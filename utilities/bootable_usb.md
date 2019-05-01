# Create a bootable usb on linux machine


## Creation
* check the usb device 
`sudo fdisk -l`

let's presume it is */dev/dbh* 

* unmount it
`sudo umount /dev/dbh`

* flash it
`sudo dd if=my.iso of=/dev/dbh bs=4M`

* it is done

## Testing

* install qemu 
`sudo apt install qemu`

* run the usb drive
`sudo qemu-system-x86_64 -hda /dev/dbh`
