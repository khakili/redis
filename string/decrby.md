## DECRBY

- 命令格式

```redis
DECRBY key decrement
```

- 描述

> 将键 key 储存的整数值减去减量 decrement 。

> 如果键 key 不存在， 那么键 key 的值会先被初始化为 0 ， 然后再执行 DECRBY 命令。

> 如果键 key 储存的值不能被解释为数字， 那么 DECRBY 命令将返回一个错误。