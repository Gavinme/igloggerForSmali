
# igloggerForSmali

将igloogger.smali放于smali文件夹根目录，在合适的位置插入下列代码。

- 打印异常栈信息

`invoke-static {}, Liglogger;->stacktrace()I  `

- 打印字符串

`invoke-static {v0}, Liglogger;->d([Ljava/lang/String;)I  `

- 打印对象

`invoke-static {v0}, Liglogger;->d(Ljava/lang/Object;)I `


以上为常用方法，剩余方法请查看源码。
