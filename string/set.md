## SET

- 命令格式

```redis
SET key value [EX seconds] [PX milliseconds] [NX|XX]
```

- 描述

> 将字符串值 value 关联到 key，会覆盖已经存在的key-value。

**当 SET 命令对一个带有生存时间（TTL）的键进行设置之后， 该键原有的 TTL 将被清除。**




- 可选参数

> [EX seconds] 设置过期时间（秒），同 SETEX key seconds value

> [PX milliseconds] 设置过期时间（毫秒），同 PSETEX key milliseconds value 

> [NX] 只有当key不存在的时候才设置值，同 SETNX key value

> [XX] 只有key存在的时候才进行操作