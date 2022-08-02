# JMX_PostgreSQL_random_table

1 таблица:
id, first_name, last_name, email

code:
INSERT INTO info_user VALUES ('${__counter(FALSE,)}', 
'${__RandomString(4,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(7,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(${__Random(3,9,)},abcdefghijklmnopqrstuvwxyz,)}@${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}.${__RandomString(${__Random(2,3,)},abcdefghijklmnopqrstuvwxyz,)}');




2 таблица:
id, id_2_table, first_name, last_name, passport_data, phone


code:
INSERT INTO info_pass VALUES ('${__counter(FALSE,)}', 
'${__counter(FALSE,)}', 
'${__RandomString(4,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(7,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(4,012345689,)} ${__RandomString(6,012345689,)}', 
'89${__RandomString(9,012345689,)}');




3 таблица:
id,  login, password, email, creation_date, id_2_table, id_3_table

code:
INSERT INTO info_pass VALUES ('${__counter(FALSE,)}', 
'${__counter(FALSE,)}', 
'${__RandomString(4,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(7,abcdefghijklmnopqrstuvwxyz,)}', 
'${__RandomString(4,012345689,)} ${__RandomString(6,012345689,)}', 
'89${__RandomString(9,012345689,)}');
