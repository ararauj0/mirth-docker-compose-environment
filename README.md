# Description

Configuration for starting projeto Mirth Connect with Database Postgres

## Requisition

- Docker
- docker-compose

## Start Project

```bash
docker-compose down -v && docker-compose up -d
```

#### Environment for services Database and Mirth Connect

|       NAME        |        Environment        |                Description                |
| :---------------: | :-----------------------: | :---------------------------------------: |
|   MIRTH_DB_HOST   |            db             |    Name of services in docker-compose     |
|   MIRTH_DB_PORT   |           5432            |             Port of Postgres              |
|   MIRTH_DB_NAME   |           mirth           |          Name of Database Mirth           |
| MIRTH_DB_USERNAME |          123456           | Username of mirth for connection Database |
| MIRTH_DB_PASSWORD |          123456           | Password of mirth for connection Database |
|    IMAGE_MIRTH    | nextgenhealthcare/connect |       Image of Mirth in Docker Hub        |
|  IMAGE_POSTGRES   |         postgres          |      Image of Postgres in Docker Hub      |
|  MIRTH_VMOPTIONS  |         Xmx3064m          |           Max of Memory in JVM            |
|        LOG        |   /tmp/pacs/mirth/logs    |             Location to save              |
|      APPDATA      | /tmp/pacs/mirth/app-data  |             Location to save              |
|       CONF        |   /tmp/pacs/mirth/conf    |             Location to save              |
|     DATABASE      |   /tmp/pacs/storage/db    |             Location to save              |

![](https://i.imgur.com/5uEi8qK.png)
