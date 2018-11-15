### Backup
    influxd backup -database metric ./data
### Restore
    influxd restore -database metric -metadir /var/lib/influxdb/meta -datadir /var/lib/influxdb/data ./data

### Note: Restart influxDB to take effect
    sudo service influxdb restart
    
#### -database - 数据库名称
#### -metadir - InfluxDB 存放元数据目录的目录，可以查看 /etc/influxdb/influxdb.conf 配置查阅
#### -datadir - InfluxDB 存放真正数据的目录，可以查看 /etc/influxdb/influxdb.conf 配置查阅

