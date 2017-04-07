# android-serial-monitor-development

## Start desktop

```
docker-compose up -d
```

## SSH

```
docker-compose run desktop sh -c "mkdir -p ~/.ssh && echo `cat ~/.ssh/id_rsa.pub` > ~/.ssh/authorized_keys"
ssh -p 4848 -D 3128 alpine@localhost
```

## RDP

```
rdp://localhost:3389 (alpine/alpine)
```
