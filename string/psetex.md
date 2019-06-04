## PSETEX

- 命令格式

```redis
PSETEX key milliseconds value
```

- 描述

> 这个命令和 SETEX 命令相似， 但它以毫秒为单位设置 key 的生存时间， 而不是像 SETEX 命令那样以秒为单位进行设置。