# liunx命令

1. 显示日期的指令： date

2. 显示日历的指令：cal

3. 简单好用的计算器：bc   (bc预设仅输出整数，如果要输出小数点下位数，那么就必须要执行 scale=number ,number就是小数点位数)

4. 重要的几个热键[Tab] (命令补全但不档案补齐),[ctrl]-c (停止当前程序), [ctrl]-d(键盘输入结束(End Of File, EOF或End OfInput))

5. Man  当你需要查看某个命令的参数时不必到处上网查找，只要man一下即可。

6. 数据同步写入磁盘： sync

输入sync，在内存中尚未被更新的数据，就会被写入硬盘中，所以，这个命令在系统关机后重新启动前，最好多执行几次！

7. 惯用的关机指令：shutdown

此外，需要注意的是，时间参数请务必加入指令中，否则shutdown会自动跳到 run-level 1 (就是单人维护的登入情况) 

重启，关机： reboot, halt , poweroff

8. 切换执行等级： init

Linux共有七种执行等级：run level 0 :关机    run level 3 :纯文本模式   run level 5 :含有图形接口模式   run level 6 :重新启动

9. 改变文件的所属群组：chgrp

10. 改变文件拥有者：chown(可修改群组的名称)

11. 改变文件的权限：chmod(数字或者是符号)

12. 变换目录：cd

13. 显示当前所在目录：pwd

14. 建立新目录：mkdir

15. 删除『空』的目录：rmdir

16. 档案与目录的显示：ls

17. 复制档案或目录：cp

18. 移除档案或目录：rm

19. 移动档案与目录，或更名：mv

20. 取得路径的文件名与目录名：basename，dirname\21. 由第一行开始显示档案内容：cat

21. 从最后一行开始显示：tac（可以看出 tac 是 cat 的倒着写）

22. 观察文件类型：file

23. 显示的时候，顺道输出行号：nl

24. 一页一页的显示档案内容：more

25. 与 more 类似，但是比 more 更好的是，他可以往前翻页：less

26. 只看头几行：head

27. 只看尾几行：tail

28. 以二进制的放置读取档案内容：od

29. 修改档案时间或新建档案：touch

30. 档案预设权限：umask

31. 配置文件档案隐藏属性：chattr

32. 显示档案隐藏属性：lsattr

33. 寻找【执行挡】：which

34. 寻找特定档案：whereis

35. 寻找特定档案：locate

36. 寻找特定档案：find

37. 压缩文件和读取压缩文件：gzip(压缩率gzip一般比zip高)，zcat

38. 压缩文件和读取压缩文件：bzip2，bzcat

39. 压缩文件和读取压缩文件：tar(压缩率100%，主要是永远打包)

zip

-r: zip -r myfile.zip ./*(将当前目录下的所有文件和文件夹全部压缩成myfile.zip文件,－r表示递归压缩子目录下所有文件.)

unzip

unzip -o -d /home/sunny myfile.zip(把myfile.zip文件解压到 /home/sunny/)

-o:不提示的情况下覆盖文件；

-d:-d /home/sunny (指明将文件解压缩到/home/sunny目录下)

zip 命令：

zip test.zip test.txt(它会将 test.txt 文件压缩为 test.zip ，当然也可以指定压缩包的目录，例如 /root/test.zip)

unzip test.zip(它会默认将文件解压到当前目录，如果要解压到指定目录，可以加上 -d 选项)

\# unzip test.zip -d /root/

40. vi

编辑文件夹  vi 文件名   vi  +行号  文件名   vi +词  文件名

编辑多个文件夹     vi  文件1  文件2

q             退出vi

q!            退出vi，不保留所做修改

wq文件夹     执行w后执行q命令 

wq!文件名     忽略w命令之前所做检查

x文件夹        做过修改的文件未写出去，该命令就把缓冲区内容写出去，然后退出vi

41. 保存并退出wq