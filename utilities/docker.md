# Docker tips and tricks

# Clean up and reclaim space 
* system purne
`docker system purne --all`

* remove dangling images
`docker rmi $(docker images --filter "dangling=true" -q --no-trunc)`

