# dockerを利用したpostgresSQLインストール

```
docker-compose up -d

docker exec -it {CONTAINER ID} /bin/bash

useradd -m -d /home/postgres postgres

passwd postgres

su - postgres

wget https://ftp.postgresql.org/pub/source/v14.6/postgresql-14.6.tar.gz

tar xzvf postgresql-14.6.tar.gz

cd postgresql-14.6

./configure --without-readline --without-zlib --prefix=/home/postgres/pgsql

make
```

