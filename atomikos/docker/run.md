### first mysql databse
```
docker run --name docker-mysql -e MYSQL_ROOT_PASSWORD=123456 -p 3333:3306 -d mysql
```

### second mysql datasource
```
docker run --name docker-mysql-2 -e MYSQL_ROOT_PASSWORD=123456 -p 3334:3306 -d mysql
```

### init

```
create database demo;
create table user_info
(
user_id     varchar(64)          not null primary key,
username    varchar(100)         null ,
age         int(3)               null ,
gender      tinyint(1)           null ,
remark      varchar(255)         null ,
create_time datetime             null ,
create_id   varchar(64)          null ,
update_time datetime             null ,
update_id   varchar(64)          null ,
enabled     tinyint(1) default 1 null
);
```
### remark
```
msyql account:root
mysql password:123456
```

