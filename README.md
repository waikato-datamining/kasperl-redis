# kasperl-redis
Base-classes for [Redis](https://redis.io/) plugins to be used in 
[kasperl](https://github.com/waikato-datamining/kasperl)-based frameworks.


## Installation

Via PyPI:

```bash
pip install kasperl_redis
```

The latest code straight from the repository:

```bash
pip install git+https://github.com/waikato-datamining/kasperl-redis.git
```


## Classes

### Core

* kasperl.redis.core.RedisSession: for storing the current Redis session

### Reader

* kasperl.redis.reader.AbstractRedisReader: base class for Redis-based readers
* kasperl.redis.reader.AbstractRedisListener: ancestor for readers that listen on a channel for incoming data

### Filter

* kasperl.redis.filter.AbstractRedisFilter: base class for Redis-based filters
* kasperl.redis.filter.AbstractRedisPubSubFilter: ancestor for filters that listen for data (sub) and push out the filter data (pub) 

### Writer

* kasperl.redis.writer.AbstractRedisWriter: base class for Redis-based writers
* kasperl.redis.writer.AbstractRedisBroadcaster: ancestor for writers that broadcast the incoming data
