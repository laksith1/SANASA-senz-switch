#N.B  This is the customized version of senzprojects/udp-switch for SANASA projects

# Setup with docker

## Build docker images
```
docker build --tag senz/switch .
```

## Run dockerize switch 
```
docker build --tag senz/switch .
docker run -it -d -p 9090:9090/udp -v /home/wasn/sdbl/switch/logs:/app/senz/logs senz/switch
```

## Virtualbox port forwarding rules boot2docker(for OS-X or Windows)
```
VBoxManage controlvm "boot2docker-vm" natpf1 "udp-port9090,udp,,9090,,9090";
```
