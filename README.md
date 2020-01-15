# Node Auth 1 Guided Project

Guided project for **Node Auth 1** Module.

## Prerequisites

- [DB Browser for SQLite](https://sqlitebrowser.org) installed.

## Project Setup

- [ ] fork and clone this repository.
- [ ] **CD into the folder** where you cloned **your fork**.
- [ ] type `npm i` to download dependencies.
- [ ] type `npm run server` to start the API.

Please follow along as the instructor adds authentication to the API.


NOTES
These two mean two different things and should not be confused
Authentication/Authn == Who are you?
Autherization/Authz == what do you want?

Authentication core principles:
-require strong password
    -
-properly sroring passwords
-preventing brute-force attacks

hashing 
----------
hash("hello world") === "jkdjahfhuoeawhfy7rnojahuyhfuewnfouhaew78"

cryptographic hashing

[rainbow table]
md5_hash                              associated_password
---------------------------------------------------------------
hacker will create a table to match the md5 with the table.

another way to stop hacker is to slow down the md5. and way we can do that is to introduce something call a time complexity. this would hash the password over and over again in order to slow it down. this will slow down the hacker from days to years. 

Key derviation function 
-------------------------
hash + time == new hash which is a function that gives us a hash devvirve from antoher hash

Bcrypt is a key derivation libraby