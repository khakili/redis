## GETRANGE

- 命令格式

```redis
//GETRANGE 命令在 Redis 2.0 之前的版本里面被称为 SUBSTR 命令。
GETRANGE key start end
```

- 描述

> 返回键 key 储存的字符串值的指定部分， 字符串的截取范围由 start 和 end 两个偏移量决定 (包括 start 和 end 在内)。

> 负数偏移量表示从字符串的末尾开始计数， -1 表示最后一个字符， -2 表示倒数第二个字符， 以此类推。

> GETRANGE 通过保证子字符串的值域(range)不超过实际字符串的值域来处理超出范围的值域请求，也就是说end最大为字符串的长度