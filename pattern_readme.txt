python pattern.py create 150  来生成一串测试用的150个字节的字符串
一般输入输入创建的字符串之后会产报错，有如下的一段错误:
	Program received signal SIGSEGV, Segmentation fault.
	0x37654136 in ?? ()
然后再使用下面这条命令:
	python pattern.py offset 0x37654136
就会计算出pc返回点的覆盖字节数
	hex pattern decoded as: 6Ae7
	140
