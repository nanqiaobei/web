# CSS
CSS中文称为层叠样式表，用来控制网页数据的表现，可以使网页的表现与数据内容分离。<br>
## 1.行列式   直接不推荐使用<br>
## 2.嵌入式嵌入式是将CSS样式集中写在网页的<head></head>标签对的<style></style>标签对中。格式如下：<br>
<head><br>
    <meta charset="UTF-8"><br>
    <title>Title</title><br>
    <style><br>
        p{<br>
            background-color: #2b99ff;<br>
        }<br>
    </style><br>
</head><br>
## 3 链接式 将一个.css文件引入到HTML文件中<br>
<link href="mystyle.css" rel="stylesheet" type="text/css"/><br>
## 4.导入式<br>
 将一个独立的.css文件引入HTML文件中，导入式使用CSS规则引入外部CSS文件，<style>标记也是写在<head>标记中，使用的语法如下：<br>    
<style type="text/css"><br>
         >>>>> @import"mystyle.css"; 此处要注意.css文件的路径<br>
</style><br>　
注意： 导入式会在整个网页装载完后再装载CSS文件，因此这就导致了一个问题，如果网页比较大则会儿出现先显示无样式的页面，闪烁一下之后，再出现网页的样式。这是导入式固有的一个缺陷。使用链接式时与导入式不同的是它会以网页文件主体装载前装载CSS文件，因此显示出来的网页从一开始就是带样式的效果的，它不会象导入式那样先显示无样式的网页，然后再显示有样式的网页，这是链接式的优点。<br>
#Django
django 安装 conda install django  <br>
django 创建项目  django-admin startproject 项目名<br>
创建好一个django就是创建好了一个了一个网站：通过命令 python manage.py runserver 进行启动：：默认端口127.0.0.1：8000  可以指定端口8080<br>
