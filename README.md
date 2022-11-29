
# Hadoop Docker

## Supported Hadoop Versions
See repository branches for supported hadoop versions

## Quick Start

To deploy an example HDFS cluster, run:
```
  docker-compose up -d
```

копируем файл в корень контейнера namenode

```shell
 docker cp test.txt namenode:/ 
```

подключаемся к контейнеру namenode

```shell
docker exec -it namenode /bin/bash
```

как положить файл в HDFS

```shell
hdfs dfs -put test.txt /
```

чтение файла

```shell
hdfs dfs -cat /test.txt

```