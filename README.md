# Home Assistant Config Repo

Personal config files of our [Home Assistant](https://www.home-assistant.io) install

## 1. Create and Fill in secrets.yaml
```sh
chopper_mac: XX-XX-XX-XX-XX-XX
chopper_ip: ###.###.###.###
babymon_ip: ###.###.###.###
babymon_username: <username>
babymon_password: <password>
```

## 2. Docker-compose startup
From [HA docs](https://www.home-assistant.io/docs/installation/docker/#docker-compose):

### Start the container with:
```sh
docker-compose up -d
```
### To restart Home Assistant when you have changed configuration:
```sh
docker-compose restart
```
### To update your docker-compose image to the latest version and restart:
```sh
docker-compose pull
docker-compose up -d --build homeassistant
```
