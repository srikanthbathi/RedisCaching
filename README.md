# RedisCaching

@CachPut -- this is used in update method to update the cache.
@CacheEvict -- is used in delete method to delete an object from cache
@Cacheable --  we will use in get by keymethod to get an object from cache.
@CacheConfig



redis-cli -- to start redis in command line.
flushall -- > to delete all the keys from redis;
keys *;

unless = "#result.followers < 12000"  ---> will store only user result.followers < 12000;

**publish subscriber**


HSET -- > hash data type.

HSET {hashsetName} {Key} {Value}[value can be any object].

HGET {hashsetName} {Key} -- will return the {Value} corresponding to the given {Key}.

HGETALL {hashsetName} -- get all the key values.

HLEN {hashsetName} -- > length of keyset.

HKEYS {hashsetName}  --- > get all the keys from {hashSetName}.

HVALS {hashsetName}  -- >  get all the value from {hashSetName}

HMGET {hashsetName} {key1} {key2} ...  ->  will return all the values corresponding to the given keys.

HMSET {hashsetName} {Key1} {Value1} {Key2} {Value2}{Key3} {Value3} ....
Sets multiple hash fields to multiple values


REDIS Transaction is initiated by MULTI and then add the Set of statements that has to be atomic and Pass EXEC.
redis 127.0.0.1:6379> MULTI 
OK 
redis 127.0.0.1:6379> SET tutorial redis 
QUEUED 
redis 127.0.0.1:6379> GET tutorial 
QUEUED 
redis 127.0.0.1:6379> INCR visitors 
QUEUED 
redis 127.0.0.1:6379> EXEC  
1) OK 
2) "redis" 
3) (integer) 1 





Redis DISCARD command flushes all previously queued commands in a transaction and restores the connection state to normal.




https://dzone.com/articles/integrate-redis-to-your-spring-project

