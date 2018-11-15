### Backup
influxd backup -database metric ./data
### Restore
influxd restore -database metric -metadir /var/lib/influxdb/meta -datadir /var/lib/influxdb/data ./data

### Note: Restart influxDB to take effect
sudo service influxdb restart
