# Running this on Synology
Steps: 
- create unifi user and group
- adjust UID en GID to  999 (edit /etc/passwd and /etc/group)
- pick a location for storing settings/logs/etc (eg. /volume1/docker/unifi)
- adjust volumes in docker-compose to the location you just picked
- you need to create all subdirs bound in the docker-compose under /volume1/docker/unifi (log, db, etc.)
- docker-compose pull && docker-compose up -d # in the docker-compose.yml directory
