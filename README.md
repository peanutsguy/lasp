# LASP Server | Ubuntu + Apache2 + SQLite + PHP

# Usage
```docker
docker run -d -e TZ=America/Mexico_City -p 8080:80 -v {site_files}:/var/www/html -v {apache_config}:/etc/apache2/apache2.conf --name lasp peanutsguy/lasp
```

| Parameter | Description |
| - | - |
| -e TZ=America/Mexico_City | Timezone |
| -p 8080:80 | Listening on host port 8080 |
| -v {site_files}:/var/www/html | Mount and serve a local website |
| -v {apache_config}:/etc/apache2/apache2.conf | Local configuration file apache2.conf |