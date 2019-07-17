# Check your mysql dump with docker

```bash
# clone et set up
$ git clone https://github.com/mleralec/check-your-mysql-dump
$ cd check-your-mysql-dump

$ cp /you-dump.sql ./data/dump.sql

# run containers
$ docker-compose up -d
$ docker exec -it check-your-dump-mysql bash

$ mysql -u user -p database < /home/dump.sql
# check password in env file
```

### go to localhost:7777


> To make a dump:
>
> mysqldump -u user -p database > /home/new-dump.sql
