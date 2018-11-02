# django框架学习
## 创建项目
打开Anaconda Prompt，cd 到一个你想放置你代码的目录，然后运行以下命令：
```
django-admin startproject jsite
```
## 创建数据库
打开PyCharm，新建project，目录输入刚创建的jsite，忽略非空目录提示，直接点Yes。打开Terminal窗口，运行以下命令：
```
python manage.py migrate
```
## 运行用于开发的简易服务器
Terminal窗口中运行以下命令：
```
python manage.py runserver
```
浏览器打开[http://127.0.0.1:8000/](http://127.0.0.1:8000/)，看到“The install worked successfully! Congratulations!”字样说明成功。
## 设置语言和时区
编辑`settings.py`文件，设为简体中文和北京时间：
```
LANGUAGE_CODE = 'zh-hans'

TIME_ZONE = 'Asia/Shanghai'

USE_I18N = True

USE_L10N = True

USE_TZ = True
```
## 设置邮箱
编辑`settings.py`文件，添加邮箱设置：
```
EMAIL_HOST = 'smtp.163.com'
EMAIL_HOST_USER = 'bluejack86@163.com'
EMAIL_HOST_PASSWORD = '邮箱的授权码而非密码'
EMAIL_PORT = 465
EMAIL_USE_SSL = True
```
