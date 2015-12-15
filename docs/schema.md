# Schema Information

## projects
column name  | data type | details
-------------|-----------|-----------------------
id           | integer   | not null, primary key
title        | string    | not null
description  | text      | not null
owner_id     | integer   | not null, foreign key (references users), indexed
field_id     | integer   | not null
significance | text      | not null, length: maximum: 5000
subfield     | string    |


## media_urls
column name  | data type | details
-------------|-----------|-----------------------
id           | integer   | not null, primary key
link         | string    | not null
media_type   | string    | not null
project_id   | integer   | not null, foreign key

## publications
column name  | data type | details
-------------|-----------|-----------------------
id           | integer   | not null, primary key
title        | string    | not null
link         | string    |
project_id   | integer   | not null, foreign key


## tags
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null

## taggings
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null
project_id  | integer   | not null, foreign key (references projects), indexed, unique [tag_id]
tag_id      | integer   | not null, foreign key (references tags), indexed

## follows
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
project_id  | integer   | not null, foreign key (references projects), indexed
user_id     | integer   | not null, foreign key (references users), indexed

## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
username        | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique
