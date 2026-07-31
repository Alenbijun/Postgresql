relation db -> tables
tables connected using relatonships

users table
posts table
comments table

1 post -> 1 user
1 comment -> 1 post

1 user -> many posts

non relational db -> doesnt organise data using connected tables
documents, key value pairs

data clear struc, relationships, transactions, joins,
strong validation at db level

banking app, ecommerce,CRM

non rela - data changes very often, docs independent , not much joins

psql -U postgres -d postgres -f part1\01_first_database.sql
 psql -U postgres -d postgresql_part1
$env:PGPASSWORD = "Alenkutten"   //in terminal 

select current_database();
select current_user;
select version();
 \l  - list all teh databases
 \dt  - list all tables
 exit || \q  - to exit

  basics  - custom schema
 information_schema - postgres standard metadata schema
 pg_catalog - postgres internal system schema
 pg_toast - internal storage schema for large values 
 public -  present in every database

  psql -U postgres -d postgresql_part1 -f part1\03_first_table.sql
  psql -U postgres -d postgresql_part1 