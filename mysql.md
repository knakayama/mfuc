MySQL
=====

```bash
# innodb fragmentation
$ mysql -uroot -e "SELECT TABLE_SCHEMA, SUM(data_length+index_length) / 1024 / 1024 / 1024 AS 'Size (GB)' FROM information_schema.tables WHERE table_schema = '<database>';"
# over 100MB
$ ls -lS /home/mysql/<database> | awk '$5>=100000000 {print $NF}' | xargs -I% ls -l /home/mysql/<database>/%
# slow query log
$ mysqldumpslow -s t -r <log>
```

```bash
# http://qiita.com/akichim21/items/f1b3497e97c8f7a580ba
$ mysqldump -h host -P 3306 -u user -p database_name | gzip | aws s3 cp - s3://temp/xxx.sql.gz
$ aws s3 cp s3://temp/xxx.sql.gz - | gunzip | mysql -h host -P 3306 -p test -u user
```
