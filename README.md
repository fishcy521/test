# test
```sql
-- 建表语句
create table pms_user_(
		id int ,
    user_name varchar(20) not null,
    sex char(1) ,
    birthday date DEFAULT '2000-01-31',
    create_time datetime not null
    
);

insert into pms_user_ 
		   (id,user_name,sex,create_time)
values
       (2,'李四', '男','2018-02-02 10:37:59');

alter table pms_user_
add primary key (id,user_name);
-- 删除表
drop table pms_user_;

-- 插入数据语句
insert into pms_user_ 
		   (user_name,sex,create_time)
values
       ('张三', '男','2018-02-02 10:37:59');
insert into pms_user_ 
		   (user_name,sex,birthday,create_time)
values
       ('李四', '女',null,'2018-02-02 10:37:59');

insert into pms_user_ 
		   (user_name,sex,birthday,create_time)
values
       ('王二', null,null,'2018-02-02 10:37:59');

insert into pms_user_ 
		   (id,user_name,sex,birthday,create_time)
values
       (4,'赵六', '',null,'2018-02-02 10:37:59');
insert into pms_user_ 
		   (id,user_name,sex,birthday,create_time)
values
       (5,'孙琦', ' ',null,'2018-02-02 10:37:59');

insert into pms_user_ 
		   (id,user_name,sex,birthday,create_time)
values
       (6,'孙琦', ' ',null,'2018-02-02 10:37:59');

-- 查询语句
select * from pms_user_ where sex = '';


-- hahahahahahahahahaahahahahh
```
