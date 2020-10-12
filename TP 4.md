# TP 4 

## Première Partie :

### Docker-compose.yml

```sql
version:  '3.7'

services:
    mysql:
        image: mysql:5.7
        restart: always
        environment:
            MYSQL_ROOT_PASSWORD: password
        volumes:
            - ./mysql:/var/lib/mysql
            - ./backups:/backups
```

### Cron
```cron
0 17 * * 0 PATH_FILE >/dev/null 2>&1
```
