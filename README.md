Dockerfile Redis
================

```
root@ruo91:~# docker build --rm -t ssh dockerfile-example/redis
root@ruo91:~# docker run -d -p 6379:6379 -h "redis" --name "redis" `docker images | grep redis | awk '{print $3 }'`
```
