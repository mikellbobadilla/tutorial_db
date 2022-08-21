<html>
<style> 
:root{
    --primary-title: #ffd369;
    --head-title: #f05454;
    --article-title: #21e6c1;
}
.head-title{
    color: var(--head-title)
}
.article-title{
    color: var(--article-title);
}
.title_db{
    color: var(--primary-title);
}

mark{
    color: white;
}
</style>

<mark>
<h1 class="head-title">Steps to Work on Database</h1>

<!-- # Steps to Work on Database -->

<h2 class="article-title">Installation</h2>

<h3 class="title_db">postgresql</h3>

**For Ubuntu 22-LTS**:

Is recomended to update the packages first

```bash
sudo apt update
```

Installing Postgre:

```bash
sudo apt install postgresql postgresql-contrib
```

Accessing to postgresql:

**postgres** is the user created when postgrest while installed.

**psql** is a based terminal interactive what enables for the user allows querys our database.

```bash
sudo -u postgres psql
```

now the prompt shows like this:

```bash
postgres=#
```

Now you can execute query for example

```bash
postgres=# CREATE DATABASE <nabe_db>;
```

Create User:

```bash
create user <user> with password <'pass'>;
```

Create Database:

```bash
create database <db_name> with owner <user_created>;
```

Allowing permissions a user:

```bash
alter user <user_created> with superuser;
```

<mark>
</html>