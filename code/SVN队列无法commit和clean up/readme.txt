解决方案：

1、下载sqlite3.exe放置到本地库内（与.SVN队列同级<.SVN是隐藏文件夹）

2、找到.svn目录查看内部是否有wc.db文件

3、打开cmd命令行，进入到sqlite3.exe所在的位置，执行：
	代码：sqlite3 .svn/wc.db
4丶进入到数据库了，然后查询工作列表的表；
	代码：select * from work_queue
5丶如何有一条数据没有执行完成，那么就删除这条命令；
	代码：delete from work_queue
6丶继续查看还有没有删除的队列；
	代码：select * from work_queue
7丶clean up；
