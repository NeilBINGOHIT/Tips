###Mac Tips

1. 终端说英语

		say yes

2. Spotlight 快速打开应用

	crtl + space 呼出

	command + I 给应用添加 key words 供 Spotlight 定位

3. `sips` 批处理图片

		#宽度缩小为800px，高度按比例缩放
		sips -Z 800 ~/Pictures/*.JPG

		#顺时针旋转90°
		sips -r 90 ~/Pictures/*.JPG

		#垂直反转
		sips -f vertical ~/Pictures/*.JPG

		更多命令 sips -h 查看

4. `command + I` 直接打开邮件

	使用 Safari 时 command + I 直接打开邮件并把当前网页附加到待发送邮件

5. `shift + command + delete` 清空废纸篓

	在 find 中选中文件 command + delete 删除； shift + command + delete 彻底删除；

6. `du -sh *` 获悉目录空间

7. esc 英文自动完成

8. `command + O` 打开文件夹

9. `sudo periodic daily weekly monthly` 定期维护

10. `shift + command + 3` 全屏截图

	`shift + command + 4` 区域截图

	默认格式为 png

		#设置其他格式
		defaultes write
		com.apple.screencapture type -
		string JPEG

11. 插件

	TotalFinder: Finder 增强插件，增加多标签、多面板、UI设置等 （收费）

	XtraFinder 和 TotalFinder 类似 （免费开源）

	Breeze: 窗口管理软件 `optiong +1/2/3` 分别对应最大化、左半屏、右半屏 （收费）

	Trillian: 整合 MSN, GTalk, Twitter

	smcFanControl: 风扇控制

12. 监控

	    * top
	
	    	显示目前系统进程情况、CPU使用情况、内存使用情况、磁盘使用情况和进程的详细列表等信息
	
    	* htop
	
    		更高级的 top， 多个 CPU、内存统计、uptime，更详细的进程信息
	
    		`sudo port install htop` 安装

13. ssh copy

		#本地到远端
		scp ./ testfile.txtusername@10.0.0.1:/tmp

		#远端到本地
		scp username@10.0.0.1:/tmp/testfile.txt ./

14. Go2Shell

	通过 Finder 浏览文件夹时直接在当前目录中打开终端，支持原生终端、 iTerm2 和 xterm， 在终端输入 `open -a Go2Shell --args config` 进行配置

15. Remote Desktop Connection for mac

	微软提供的 mac 远程桌面连接 windows 工具

16. Keynote, Pages, Numbers 鼠标移至文档标题时出现小箭头，可以对文档进行版本控制


17. time 命令

	查询在终端执行的某程序耗时、对 CPU 的使用等情况

		time python fil.py

		#输出
		python fib.py0.02s user 0.02s
		system 50% cpu 0.094 total

18. F.lux 自动调节色温

19. `pmset noidle` 不休眠， 关闭终端取消命令

	`pmset` 是 OS X 提供的命令行电源管理工具，很好很强大

		#设置在2013/1/1 8:00 幻想电脑
		sudo pmset schedule wake "01/01/13 20:00:00"

20. Finder 中选中文件 space 预览

21. 复制文件目录下文件名列表

	`command + a` `command + c` 打开文件编辑器 `command + v` 就是这么简单

22. 显示/隐藏

		chflags hidden ~/Desktop/*
		chfilags nohidden ~/Desktop/*


23. Homebrew 功能和 MacPorts 很像，更为轻量，安装方便编译快，开发必备

24. 快速定位 `locate` 命令 `locate nginx.conf`

25. shift 慢速动画，效果很酷炫

26. 搜索命令 mdfind

		mdfind xindervella
		mdfind -onlyin ~/Desktop xindervella
		mdfind -count -onlyin ~/Desktop xindervella
		mdfind -name xindervella

27. 生成 man page 的 pdf 文档

		man -t grep | open -f -a Preview

28. 去除右键菜单重复项

		/System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -kill -r -domain local -domain system -domain user

29. Scroll Reverser 实现鼠标和触摸板的分别设置

30. Retinilizer 把非 retina 软件 retina 化

31. `vimdiff destfile.tet sourcefile.txt` 普通文件对比

	VisualDiffer （收费 25 RMB）UI、功能和稳定性都不错，实在是居家旅行、代码比较、查找问题的必备利器

32. option + command + esc 强制关闭

33. Cheat-Sheet 按住 command 两秒 弹出一个当前应用的快捷键列表

34. HTML5 Player

	mac 一直对 Flash 很抵触，支持也不好，播一会就会很热，而且某酷、某豆的广告太多、页面混乱也不适合观看。于是某位无聊程序员做了一个 HTML5 播放器， [HTML5 Player](http://zythum.sinaapp.com/youkuhtml5playerbookmark/)

35. 重建 Spotlight 索引

		sudo mdutil -i off /
		sudo mdutil -E /`
		sudo mdutil -i on /`




