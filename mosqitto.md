# Mostitto

## run mosquitto using docker
```
docker run -it --rm -p 1883:1883 -p 9001:9001 -v /mosquitto:/mosquitto eclipse-mosquitto
```

## edit config
```
vi /mosquitto/config/mosquitto.conf
listener 1883
allow_anonymous true
persistence true
persistence_location /mosquitto/config/data/
log_dest file /mosquitto/config/xx.log
log_dest stdout
#log_dest none
log_type all
```
