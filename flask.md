## 安装Flask框架并且在PyCharm中配置虚拟环境

### 安装Flask框架

第一步：打开终端,输入cmd 回车打开命令行

```
win + R 打开运行框
```
<img src="https://github.com/what1115/2024python/blob/main/img/img_1.png">
<img src=".\img\img_1.png">

第二步：在终端中输入以下命令创建虚拟环境

```
virtualenv "虚拟环境名称"
```
<img src=".\img\img_2.png">

出现
<img src=".\img\img_3.png">
则创建成功
二： 使用虚拟环境

```
D:\env>.\flask_env\Scripts\activate   # “flask_env” 是虚拟环境名称
```
出现

<img src=".\img\img_4.png">

则激活成功

三：安装Flask框架

输入pip install Flask命令安装Flask框架
```
(flask_env) D:\env>pip install Flask
```
出现下图则安装成功

<img src=".\img\img_5.png">

### 在pycharm中配置虚拟环境

打开PyCharm，点击菜单栏File -> New project ->

<img src=".\img\img_6.png">

点击创建

新建一个app.py文件，

<img src=".\img\img_7.png">
<img src=".\img\img_8.png">
<img src=".\img\img_9.png">

配置python解释器(选择刚才创建的虚拟环境)

输入以下代码

```
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, World!'


if __name__ == '__main__':
    app.run()
```

<img src=".\img\img_11.png">

运行app.py文件
```
Shift + F10
```

出现

<img src=".\img\img_10.png">

则运行成功

打开浏览器
输入

```
http://127.0.0.1:5000/
```

<img src=".\img\img_12.png">

回车后出现

<img src=".\img\img_13.png">

### 完成第一个Flask程序开发
