# AnimusDocker

## Dolibarr ERP
![image](https://github.com/xschahl/AnimusDocker/assets/91027790/b4f1d71d-42b3-4536-b91d-0244af557989)

### Lancement de l'application
``` 
cd dolibarr
```
```
sudo docker-compose up -d
```

### Accéder à l'application
http://0.0.0.0

## Dokuwiki
![image](https://github.com/xschahl/AnimusDocker/assets/91027790/cc17b34c-5d5c-4755-934f-f2cb7296dfbe)

### Installer l'application
```
docker exec -it dokuwiki /bin/bash
```
```
cd /var/www/html
curl --remote-name https://download.dokuwiki.org/src/dokuwiki/dokuwiki-stable.tgz
tar -xzvf dokuwiki-stable.tgz --strip-components=1
rm dokuwiki-stable.tgz
chown -R www-data:www-data /var/www/
```

### Lancement de l'application
``` 
cd dokuwiki
```
```
sudo docker-compose up -d
```

### Accéder à l'application
http://localhost:8888
