# NOTES

## Influxdb v1.8

This will not work with 2.x
```bash
# Create a backup in the portable format
influxd backup -portable /path/to/backup-destination

# Restore from a portable backup
influxd restore -portable /path/to/backup-destination
```


## Mosquitto
```bash
allow_anonymous true  # allows connection outside of localhost
listener 1883
password_file /mosquitto/config/cred
```

password file has to be created on the running docker container
```bash
mosquitto_passwd -c /mosquitto/config/cread <username>
```

