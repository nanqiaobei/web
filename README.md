
# Django
django 安装 conda install django  <br>
django 创建项目  django-admin startproject 项目名<br>
创建好一个django就是创建好了一个了一个网站：通过命令 python manage.py runserver 进行启动：：默认端口127.0.0.1：8000  可以指定端口8080<br>
## Django程序目录 
manage.py 对当前Django程序所有操作都是通过这个操作的<br>
-settints.py Django配置文件<br>
-url.py  路由系统：url->函数<br>
-wsgi.py  用于定义 Django 用socket,wsgiref,uwsgi<br>


# 关于没有template这个文件
需要到setting.py文件中去设置：TEMPLATES 字典中，列表里面加上：os.path.join(BASE_DIR,"templates“) 其中BASE_DIR 为文件夹的路径<br>
# 关于配置静态文件
在STATIC_URL='/static/'下面添加：<br>
STATICFILES_DIRS=(os.path.join(BASE_DIR,'自己定义的文件名’)),然后在文件连接中需要用到static这个最为前缀,最简单的做法是定义文件时候全部用法static<br>
