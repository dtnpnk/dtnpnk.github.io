# DOCKER - Cheatsheet

## deletes old containers  and images

```bash
docker ps -a | grep "Exit-Created" | cut -d ' ' -f 1 | xargs sudo docker rm; docker images | grep "<none>" | awk '{print $3}' | xargs sudo docker rmi
```



