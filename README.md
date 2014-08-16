Dockerfile Redis
================
- Build
```
root@ruo91:~# git clone https://github.com/ruo91/docker-redis /opt/docker-redis
root@ruo91:~# docker build \
--rm -t redis:stable /opt/docker-redis
```
- Run
```
root@ruo91:~# docker run \
-d --name="redis" -h "redis" -p 6379:6379 redis:stable
```
