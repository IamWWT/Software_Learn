VScode 入门。

学习网站：https://code.visualstudio.com/docs#vscode

我的目的：python, c/c++ 代码的运行【轻量代码下】。

1. vscode + tensorflow
 1.1 配置python的路径。搜索python.pythonPath.
	要使用TensorFlow，则配置tensorflow所安装在的那个环境的python路径。
	打开vscode的【文件】-【首选项】-【设置】，快捷键"Ctrl+,"。设置Python的路径
	// 将设置放入此文件中以覆盖默认设置
	{
		"python.pythonPath": "D:/PACKAGE/Anaconda3/envs/Scripts", //配置自己python路径
		"python.linting.flake8Enabled": true, 
		"python.linting.pylintEnabled": false,
		//"python.linting.pylintArgs": ["--disable-msg=C0103"],
		"python.formatting.provider": "yapf"
	}
	
通过Anaconda安装tensorflow时，一般会新建一个虚拟环境(env)，但是vscode在调试python代码时默认使用的是base环境下的路径，这就会出现无法解析tensorflow的情况。所以需要将tensorflow环境的路径添加到vscode的settings.json用户设置中，即可在vscode中搭建TensorFlow的开发环境。

新开.py文件打开即可选择环境运行代码。

2. 几点说明。
配置yapf: pip install yapf后，在VScode中 按Alt+Shift+F即可自动格式化代码。
配置flake8：pip install flake8后，vscode的settings.json文件中，输入 python.linting.flake8Enabled:True 即可，该功能可以在写代码的时候编辑器提示哪里出错，哪里格式不规范。
查看函数或者类的定义：Ctrl+鼠标左键点击函数名或者类名，OR，在函数名或者类名上按F12也可。
变量名上，按F12即可实现重命名变量。
断点调试：行号左边点击设置断点，左侧调试界面看变量的变化。

3. launch.json对应配置中，添加一行： 
"console":"none"
# none 只输出到调试控制台
# integratedTerminal  同时输出到“调试控制台”和软件内置的“终端”
# externalTermimal 输出到外部”终端“

4. VScode里用Git.
VScode里直接集成了Git。
VScode的Git部分。

--------------------- 
https://blog.csdn.net/Briliantly/article/details/82847804 
https://www.cnblogs.com/clemente/p/10022006.html
