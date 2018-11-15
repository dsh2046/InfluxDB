influxd backup -database metric ./data

influxd restore -database metric -metadir /var/lib/influxdb/meta -datadir /var/lib/influxdb/data ./data
