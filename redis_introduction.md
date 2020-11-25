# Introduction to Redis


Redis is an in memory database that is fast in nature since it loads and stores the data in the Random Access Memory.


## Intallation

To install it in Ubuntu:

```
$ sudo apt install redis-server
```


The service can be enabled on system startup with:

```
$ sudo systemctl enable redis-server
```

Or just start it without loading it as a startup program:

```
$ sudo systemctl start redis-server
```


To verify the status of the server:

```
$ sudo systemctl status redis-server.service
```

Enable redit as a systemd service by changing the file at "/etc/redis/redis.conf", just add the 
following line: "supervised systemd".


## Introduction

The redis shell can be launched using the __redis-server___ _just run it in the terminal:

```
$ redis-cli
```

Default configuration can be seen by typing: "config get \*".

Configuration variables can be changed with the _set_ command:

```
127.0.0.1:6379> config set requirepass "password"
```


## Persistence

Persistence can be achieved using storing the data in:
+ disk
+ log file


