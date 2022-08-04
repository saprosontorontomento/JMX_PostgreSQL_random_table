# JMX_PostgreSQL_random_table

# 1 таблица:
```
first_name
last_name
email
```
```
INSERT INTO info_user (first_name,last_name,email) VALUES ('${__RandomString(4,abcdefghijklmnopqrstuvwxyz,)}',
'${__RandomString(7,abcdefghijklmnopqrstuvwxyz,)}',
'${__RandomString(${__Random(3,9,)},abcdefghijklmnopqrstuvwxyz,)}@${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}.${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}');
```
# 2 таблица:
```
first_name
last_name
pass_num
phone
```
```
INSERT INTO info_pass (first_name,last_name,pass_num,phone)  VALUES ('${__RandomString(4,abcdefghijklmnopqrstuvwxyz,)}',
'${__RandomString(7,abcdefghijklmnopqrstuvwxyz,)}',
'${__RandomString(4,012345689,)} ${__RandomString(6,012345689,)}',
'89${__RandomString(9,012345689,)}');
```
# 3 таблица:
```
login
password
email
creation_date
```
```
INSERT INTO info_acc (login,password,email,creation_date) VALUES ('${__RandomString(10,abcdefghijklmnopqrstuvwxyz,)}',
'${__RandomString(10,abcdefghijklmnopqrstuvwxyz0123456789,)}',
'${__RandomString(${__Random(3,9,)},abcdefghijklmnopqrstuvwxyz,)}@${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}.${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}',
'${__timeShift(yyyy/MM/dd,,,,)}');
```
