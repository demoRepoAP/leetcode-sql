# Leetcode SQL Questions & Solutions <br/>

<b>Repository Contains :</b><br/>

(1) 130+ Leetcode SQL Question Solutions<br/>
(2) PostgreSQL Dump File (leetcodedb.sql)<br/>
<br/>
<b> Problem statements of all questions including leetcode premium questions :</b><br/>

(1) https://leetcode.ca/ <br/>
(2) https://lifewithdata.com/sql/<br/>
<br/>
<b>How to Import dump file using command line terminal?</b><br/>

(1) Open terminal & open psql utility
```
user@my-machine:~$ psql
```
(2) Create Database (To import the dump file, database should be created priorly)<br/>
```
postgres=# CREATE DATABASE sample_db;
```
(3) Quit the psql promt
```
postgres=# \q
```
(4) From terminal, Load dump file into the newly created database using below command
```
user@my-machine:~$ pg_restore --host "127.0.0.1" --port "5432" --username "postgres" --dbname "sample_db" --verbose "leetcodedb.sql"
```
<br/>
<b>How to Import dump file using PgAdmin tool?</b><br/><br/>

(1) Open PgAdmin & Create Database
```
Servers -> Databases -> Create -> Database.. (Create Database dialog will get opened)
```
(2) Restore Dump File<br/>
```
Right Click on newly created Database & select Restore option from menu (Restore dialog will get opened)
```
Just Browse the dump file and keep other options as it is.<br/>

<b>Notes : </b><br/>

(1) Do not just copy-paste and run the content of dump file into either "psql promt in terminal" or "query tool of pgadmin".<br/>
   (Because dump file contains COPY commands not INSERTS,So doing such will cause errors.)<br/>
(2) Replace your configurations(host,port,username) in pg_restore command<br/>
(3) Table names are suffixed with question number.<br/>
(4) New solutions will get added as I solve them.<br/>
