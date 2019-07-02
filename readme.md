
example

```
$ docker run -d -p 4444:4444 -p <port4VNC>:5900 -v /dev/shm:/dev/shm selenium/standalone-chrome-debug:3.12.0-boron
$ docker run -d -p 4444:4444 -p <port4VNC>:5900 -v /dev/shm:/dev/shm selenium/standalone-firefox-debug:3.12.0-boron

$ docker run -d -p 4444:4444 -p 5900:5900 -v /dev/shm:/dev/shm selenium/standalone-chrome-debug:3.12.0-boron

$ docker run -d -p 4444:4444 -p 5901:5900 -v /dev/shm:/dev/shm selenium/standalone-firefox-debug:3.12.0-boron

$ docker run -d -p 4450:4444 --name selenium-hub selenium/hub:3.12.0-boron
$ docker run -d -P -p 5900:5900 --link selenium-hub:hub -v /dev/shm:/dev/shm selenium/node-chrome-debug:3.12.0-boron
$ docker run -d -P -p 5901:5900 --link selenium-hub:hub -v /dev/shm:/dev/shm selenium/node-firefox-debug:3.12.0-boron
```


啟動
```
docker-compose up -d
```


連接密碼

```
secret
```




