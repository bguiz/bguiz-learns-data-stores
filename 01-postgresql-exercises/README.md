# PostgreSQL Exercises

## Set up

```bash
sudo -u postgres createuser --interactive
# name: pgexercises
# superuser: yes
sudo -u postgres createdb pgexercises
sudo -u pgexercises psql pgexercises

```

Initialise schema and data using:

https://pgexercises.com/dbfiles/clubdata.sql

## Basic

https://pgexercises.com/questions/basic/

https://pgexercises.com/questions/basic/selectall.html

```sql
SELECT * from cd.facilities;

```

https://pgexercises.com/questions/basic/selectspecific.html

```sql
SELECT name, membercost
FROM cd.facilities;

```

https://pgexercises.com/questions/basic/where.html

```sql
SELECT *
FROM cd.facilities
WHERE membercost > 0;

```

https://pgexercises.com/questions/basic/where2.html

```sql
SELECT facid, name, membercost, monthlymaintenance 
FROM cd.facilities 
WHERE membercost > 0 and membercost < monthlymaintenance * 0.02;

```

https://pgexercises.com/questions/basic/where3.html

```sql
SELECT * 
FROM cd.facilities 
WHERE name like '%Tennis%';

```

https://pgexercises.com/questions/basic/where4.html

```sql
SELECT * 
FROM cd.facilities 
WHERE facid in (1, 5);

```
