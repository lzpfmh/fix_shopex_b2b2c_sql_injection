##原因

shopex b2b2c 虽然使用了doctrine框架，但没有使用Mysql的prepare-bind方式来防止SQL注入，我做的这个工作就是修改底层DB
实现利用doctrine的setParameters方式把b2b2c直接拼SQL的方式改为安全的prepare-bind方式。


##使用方式

在二开方式替换目录