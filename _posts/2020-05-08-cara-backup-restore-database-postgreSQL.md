---
title:  "Cara Backup Restore Database PostgreSQL"
header:
  teaser: "assets/images/cara-backup-restore-database-postgresql/teaser.png"
categories: 
  - Tutorial
tags:
  - postgresql
---

Server database postgreSQL menyediakan utilitas **pg_dump** dan **psql** untuk membackup dan merestore database.Kali ini saya akan menjelaskan cara untuk menggunakan perintah **pg_dump** untuk membackup database dan **psql** untuk merestore database.


{% include toc title="Backup Dan Restore" %}

Dibawah ini adalah beberapa perintah yang digunakan untuk membackup dan merestore database PostgreSQL

* **-d, –dbname=DBNAME** nama dabatase
* **-h, –host=HOSTNAME hostname** atau ipserver PostgreSQL
* **-p, –port=PORT** server port PosgreSQL (default: 5432)
* **-U, –username=NAME** username PostgreSQL
* **-W, –password** password PostgreSQL
* **–role=ROLENAME** mengatur Role

## 1. Backup Restore Database Tertentu
### Backup Database Tertentu
```sql
$ pg_dump -U postgres -d dbname > dbname.sql
```
### Restore Database Tertentu
```sql
$ psql -U postgres -d dbname < dbname.sql
```

## 2. Backup Restore Semua Database
### Backup Semua Database
```sql
$ pg_dumpall -U postgres > alldatabase.sql
```
### Restore Semua Database
```sql
$ psql -U postgres < alldatabase.sql
```

## 3. Backup Restore Table Tertentu
### Backup Table
```sql
$ pg_dump -U postgres -d dbname-t tablename > dbname-tablename.sql

```
### Restore Table
```sql
$ psql -U postgres -d dbname < dbname-tablename.sql
```

## 4. Compressed Backup Restore Database
### Backup Database Dengan Format Compressed PostgreSQL
```sql
$ pg_dump -U postgres -d dbname| gzip > dbname.sql.gz

```
### Restore Database Dengan Format Compressed PostgreSQL
```sql
$ gunzip -c dbname.sql.gz | psql -U postgres -d dbname
```

## 5. Multiple Backup Restore Database
### Multiple Backup
```sql
$ pg_dump -U postgres -d dbname | split -b 100m – dbname.sql

```
### Multiple Restore
```sql
$ cat dbname*.sql | psql -U postgres -d dbname
```