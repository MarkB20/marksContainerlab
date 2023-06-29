# marksContainerlab 
# just testing only but will have instruction and points to troubleshooting issues

# Pre-requisites [Taken from Containerlab](https://containerlab.dev/install/)

The following requirements must be satisfied to let containerlab tool run successfully:

    A user should have sudo privileges to run containerlab.
    A Linux server/VM2 and Docker installed.
    Load container images (e.g. Nokia SR Linux, Arista cEOS) that are not downloadable from a container registry. Containerlab will try to pull images at runtime if they do not exist locally.

***********************************************************************************************************

# docker issues with linux on vm

1. you may not have it installed on your linux vm of choose this is one for debian but look it up as its easy to find [installing curl on debian](https://www.cyberciti.biz/faq/howto-install-curl-command-on-debian-linux-using-apt-get/)

2. Curl (6) error or dowload.docker not working. follow this tutarial and it hopefuly should fix the issues [ltheme curl 6 fix](https://ltheme.com/curl-6-could-not-resolve-host/)

3. **Big issue** podman will have to be unistalled for alot of people to get docker working. IBM has instutions on how to [IBM remove podman](https://www.ibm.com/docs/en/edge-computing/4.2?topic=questions-troubleshooting-tips#uninstall_podman)


***********************************************************************************************************
# links to the images used on the qick start 

1. [Nokia SR Linux](https://github.com/nokia/srlinux-container-image)
   
2. [Arista cEOS images](https://www.arista.com/en/support/software-download) will need account

***********************************************************************************************************
# IF USING THE YML ABOVE

change the name of the container in the yml file to your own container name 
***********************************************************************************************************
# container lab list of good commands 

1 starting it 
```
containerlab deploy
```

2. showing it graphically
  ```
sudo containerlab graph --topo <NAME-OF-CONF-YML>
```

3. destroying it
 ```
   containerlab destroy --topo <NAME-OF-CONF-YML>
 ```
# Docker
1. starting it
 ```
sudo systemctl start docker
 ```
