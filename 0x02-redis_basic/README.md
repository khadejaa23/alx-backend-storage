0x02. Redis basic
=================
Back-end
Redis
 By Emmanuel Turlay, Staff Software Engineer at Cruise
 Weight: 1
 
![image](https://github.com/AsuweRich/S.E_Bounty/assets/106776383/d9cfde71-7060-4f3b-a3e5-63f27cb3b4d1)

Resources
---------

**Read or watch:**

-  [Redis commands](https://redis.io/commands/ "Redis commands")
-  [Redis python client](https://redis-py.readthedocs.io/en/stable/ "Redis python client")
-  [How to Use Redis With Python](https://realpython.com/python-redis/ "How to Use Redis With Python")
-  [Redis Crash Course Tutorial](https://www.youtube.com/watch?v=Hbt56gFj998 "Redis Crash Course Tutorial")

Learning Objectives
-------------------

-  Learn how to use redis for basic operations
-  Learn how to use redis as a simple cache

Requirements
------------

-  All of your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7)
-  All of your files should end with a new line
-  A `README.md` file, at the root of the folder of the project, is mandatory
-  The first line of all your files should be exactly `#!/usr/bin/env python3`
-  Your code should use the `pycodestyle` style (version 2.5)
-  All your modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
-  All your classes should have documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`)
-  All your functions and methods should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`)
-  A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)
-  All your functions and coroutines must be type-annotated.

Install Redis on Ubuntu 18.04
----------------
```
$ sudo apt-get -y install redis-server
$ pip3 install redis
$ sed -i "s/bind .*/bind 127.0.0.1/g" /etc/redis/redis.conf
```

Use Redis in a container
----------------

Redis server is stopped by default - when you are starting a container, you should start it with: `service redis-server start`
