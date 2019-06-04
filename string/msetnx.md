## MSETNX

- 命令格式

```redis
MSETNX key value [key value …]
```

- 描述

> 当且仅当所有给定键都不存在时， 为所有给定键设置值。

> 即使只有一个给定键已经存在， MSETNX 命令也会拒绝执行对所有键的设置操作。

**MSETNX 是一个原子性(atomic)操作， 所有给定键要么就全部都被设置， 要么就全部都不设置， 不可能出现第三种状态。**

- 可选参数

> [key value …]  多个Key Value，要保证是先key，后value