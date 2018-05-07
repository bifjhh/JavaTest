>身为一个java小白，我也是第一次安装java的环境。欢迎大佬们指正

### 下载
- 首先是找下载的地址，看网上的教程先安装JDK，但是之前的比较老，找到了最新版的官方文件---
- 然后被告知官网默认下载的是jdk9 版本的， 太高了，不太适合开发
- 然后朋友得知后给了我一个连接，Java SE 的8版本，其中也包括了JDK，[点击进入下载](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- 进入后是这么一个页面，点击左边的 Java SE8 下载  选择对应的操作系统版本下载就可以了

- 下载完成后一个exe文件
    + 点击安装即可
    ![这里写图片描述](http://img.blog.csdn.net/20180128014228422?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    + 下一步 下一步 下一步 如果更改路径，请自行更改
![这里写图片描述](http://img.blog.csdn.net/20180128014322145?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
![这里写图片描述](http://img.blog.csdn.net/20180128014356726?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

- 安装完成后 开始配置环境变量

### 配置环境变量
1. 右键单击桌面计算机图标，点击“属性”
![这里写图片描述](http://img.blog.csdn.net/20180128014447969?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

2. 点击“高级系统设置
![这里写图片描述](http://img.blog.csdn.net/20180128014520786?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

3. 点击“环境变量”
![这里写图片描述](http://img.blog.csdn.net/20180128014608598?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
4. 点击  新建
	![这里写图片描述](http://img.blog.csdn.net/20180128014631326?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    + 新建变量名 输入  JAVA_HOME 
![这里写图片描述](http://img.blog.csdn.net/20180128014646835?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
 ![这里写图片描述](http://img.blog.csdn.net/20180128014730931?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
	+ 变量值输入 C:\java 点击确定（就是你jdk安装的目录路径）
![这里写图片描述](http://img.blog.csdn.net/20180128014817059?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
5. 在 系统变量 中找到Path，单击“编辑” 
![这里写图片描述](http://img.blog.csdn.net/20180128014830204?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    + 将 %JAVA_HOME%\bin; 添加到 变量值 中，单击 确定
![这里写图片描述](http://img.blog.csdn.net/20180128015118761?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
![这里写图片描述](http://img.blog.csdn.net/20180128015133241?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

- 根据朋友讲   classpath 环境变量是用来输出编译后的文件路径的，可能之后的编译会经常变更，所以不需要设置   
### 测试安装成功与否
- CMD命令下输入 java 
    + 弹出一大串代码表示成功安装了java
![这里写图片描述](http://img.blog.csdn.net/20180128015058280?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
- 输入java -version 
    + 弹出对应版本号表示成功    
![这里写图片描述](http://img.blog.csdn.net/20180128015109114?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvYmlmamhoX3Nr/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
