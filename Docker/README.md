### Create a docker version

  ```
  docker pull ubuntu:latest
  docker run --net=host -it -p 8200:8200 -p 1900:1900/udp -v /home/wisnuc/home/wisnuc:/home/:ro IMAGEID /bin/sh

  apt-get update
  apt-get -y install minidlna nano

  nano /etc/minidlna.conf
    media_dir=A,/home/music
    media_dir=P,/home/pic
    media_dir=V,/home/video
    friendly_name=helloworld
    
  service minidlna force-reload
  ```
