1.sql模式设置

> 全局模式
>
> `select @@global.sql_mode`  
> `set @@global.sql_mode='NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION'`
>
> 会话模式
>
> `select @@session.sql_mode`  
> `set sql_mode = 'NO_ZERO_DATE'`  
> `set @@sql_mode = 'ERROR_FOR_DIVISION_BY_ZERO'`  
> `set @@session.sql_mode = 'NO_AUTO_CREATE_USER'`



