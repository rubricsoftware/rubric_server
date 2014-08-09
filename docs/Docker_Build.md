Rubric Server - Docker App Installation
=======================

Based on info from:
http://competa.com/blog/2014/06/how-to-build-a-docker-image-based-on-debain-14-04-lts-with-an-nginx-webserver/
https://docs.docker.com/examples/nodejs_web_app/


sudo debootstrap trusty /root/ubuntu14LTS

sudo tar -C /root/ubuntu14LTS/ -c . | sudo docker.io import - ubuntu14LTS

