# Storage
## Local persistant volume storage 
- In Podman the local volumes are created in the home directory   
- podman volume create myvol 
- podman volume inspect myvol

## NFS
- podman volume create --driver local --opt type=nfs --opt o=addr=192.168.122.36,rw --opt device=:/nfsdata nfsvol   
    -   Run a container that uses that NFS storage.   
        -   podman run -it --name voltest2 --rm --mount source=nfsvol,target=/data nginx sh