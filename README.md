# android-serial-monitor-development

## Start desktop

```
docker-compose up -d
```

## Upload public ssh key

```
docker-compose run desktop sh -c "mkdir -p ~/.ssh && echo `cat ~/.ssh/id_rsa.pub` > ~/.ssh/authorized_keys"
```

## Start Microsoft Remote Desktop 

```
 rdp://localhost (alpine/alpine)
```
