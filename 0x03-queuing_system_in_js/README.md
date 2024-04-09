Queuing System in JS
Redis server

Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

How to run a Redis server on your machine
How to run simple operations with the Redis client
How to use a Redis client with Node JS for basic operations
How to store hash values in Redis
How to deal with async operations with Redis
How to use Kue as a queue system
How to build a basic Express app interacting with a Redis server
How to the build a basic Express app interacting with a Redis server and queue
Requirements
All of your code will be compiled/interpreted on Ubuntu 18.04, Node 12.x, and Redis 5.0.7
All of your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the js extension

learning objectives
https://github.com/redis/node-redis
https://github.com/Automattic/kue

installation:
Download, extract, and compile the latest stable Redis version (higher than 5.0.7 - https://redis.io/download/):

$ wget http://download.redis.io/releases/redis-6.0.10.tar.gz
$ tar xzf redis-6.0.10.tar.gz
$ cd redis-6.0.10
$ make
Start Redis in the background with src/redis-server
$ src/redis-server &
Make sure that the server is working with a ping src/redis-cli ping
PONG

to run client : src/redis-cli

Using the Redis client again, set the value School for the key Holberton
127.0.0.1:[Port]> set Holberton School
OK
127.0.0.1:[Port]> get Holberton
"School"
Kill the server with the process id of the redis-server (hint: use ps and grep)
$ kill [PID_OF_Redis_Server]
Copy the dump.rdb from the redis-5.0.7 directory into the root of the Queuing project.
