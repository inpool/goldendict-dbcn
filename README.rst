~~~~~~~~~~~~~~
   goldbcn
~~~~~~~~~~~~~~
goldbcn是一个在线词典，可以自动联网查询单词并缓存到本地，若查询时本地
数据库中有缓存结果，不会再次联网查询。

写这个脚本的初衷是为GoldenDict提供一个英-文查询引擎。

安装
=============

1. cd
2. git clone https://github.com/inpool/goldbcn.git

设置
=============

1. 打开goldendict，编辑 -> 词典 -> 词典来源 -> 程序 -> 添加
2. 勾选启用复选框
3. 类型： 纯文本
4. 命令行 ::

      /path/to/goldbcn/bin/lookup
      
现在，就可以使用该程序进行查词了。
当数据库中有要查的词时，会直接从数据库中返回结果。
当数据库中没有要查的词时，会自动到网上查，并将结果保存至数据库以便下次使用。
