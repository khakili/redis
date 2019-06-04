## SETEX

- 命令格式

```redis
SETEX key seconds value
```

- 描述

> 将键 key 的值设置为 value ， 并将键 key 的生存时间设置为 seconds 秒钟。

> 如果键 key 已经存在， 那么 SETEX 命令将覆盖已有的值。


