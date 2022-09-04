# Redis overview and commands <!-- omit in toc -->

## Contents <!-- omit in toc -->

- [1. Whats is Redis?](#1-whats-is-redis)
  - [1.1. Advantages](#11-advantages)
  - [1.2. Disadvantages](#12-disadvantages)
- [2. Commands](#2-commands)

## 1. Whats is Redis?

- Redis is an open-source NoSQL database designed as key-value pairs. Redis is essentially an open source NoSQL database that keeps data in memory.
- Redis, short for Remote Dictionary Server
- It positions itself more as a data structure server.
- Redis is not just a simple key-value server.
  - One of the most important differences among other alternatives is that Redis ability to store and use high level data structures

### 1.1. Advantages

- Is extremely fast because it works synchronously.
- Also, it supports many data types, it can save data both on RAM and on disk according to the configuration what you set. Since it records on the disc, it continues to work with the same data after restart.
- Also, It has many enterprise features such as Sharding, Cluster, Sentinel, Replication.

### 1.2. Disadvantages

- Since it does not work asynchronously, you may not be able to reach the performance that asynchronous alternatives reach on a single instance.
- Also, You will need RAM according to your data size.
- It does not support complex queries like relational databases.
- If a transaction receives an error, there is no return in the Redis.
- As you can see that, we have seen the Redis

## 2. Commands

- Enter into a Redis shell
  - redis-cli
- Get all keys
  - keys *
- Set key and value if type is string
  - set `<key>` `<value>` # Ex: set name Jefté
- Get value if type is string
  - get `<key>` # Ex: get name
- Get value if type is hash
  - hgetall `<key>`
- Knowing type of key
  - type `<key>`