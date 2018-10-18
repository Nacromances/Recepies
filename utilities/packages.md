# Handle packages in linux distributaions 


## Debian based
* search package providing file already installed 
`dpkg -S <file pattern>`


* search package providing file not installed yet
`sudo apt install apt-file
 apt-file update
 apt-file search <file pattern>`

* list installed packages
`dpkg -l`

## Redhat based

