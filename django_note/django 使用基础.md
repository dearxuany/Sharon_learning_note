# django 使用基础
## 安装 django
虚拟环境下使用 pip 安装
```
pip install django
```

## 创建 django 项目
### 生成项目初始目录结构
项目名为 mysite
```
django-admin startproject mysite
```
初始目录结构
```
.
└── mysite
    ├── bin
    │   └── venv_activate.sh
    ├── manage.py  # 命令行工具，django-admin 封装, 无需编辑此文件
    └── mysite
        ├── asgi.py
        ├── __init__.py
        ├── settings.py  # 默认配置
        ├── urls.py   # 映射 URL 路径到视图
        └── wsgi.py   # web 网关接口 WSGI

3 directories, 7 files
```
### setting.py 配置 
setting.py 中应用配置
```
# 调试模式，输出所有没有被程序自身捕获的异常，显示到错误页面
# 生成环境必须为 False
DEBUG = True

# 默认基础框架
INSTALLED_APPS = [
    'django.contrib.admin',  # 管理站点
    'django.contrib.auth',   # 验证框架
    'django.contrib.contenttypes',  # 内容类型跨级啊
    'django.contrib.sessions',  # 会话
    'django.contrib.messages',  # 消息机制
    'django.contrib.staticfiles',  # 静态文件管理
]

# 中间件列表
MIDDLEWARE = [
    'django.middleware.security.SecurityMiddleware',
    'django.contrib.sessions.middleware.SessionMiddleware',
    'django.middleware.common.CommonMiddleware',
    'django.middleware.csrf.CsrfViewMiddleware',
    'django.contrib.auth.middleware.AuthenticationMiddleware',
    'django.contrib.messages.middleware.MessageMiddleware',
    'django.middleware.clickjacking.XFrameOptionsMiddleware',
]

# 根 URL 路径
ROOT_URLCONF = 'mysite.urls'

# 数据库全部配置，字典格式
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}

# 默认编码
LANGUAGE_CODE = 'en-us'

# 时区
TIME_ZONE = 'UTC'

USE_I18N = True

USE_L10N = True

# 时区支持启禁用
USE_TZ = True

# 静态文件提取输出相对路径
STATIC_URL = '/static/'
```
#### 数据库
数据库配置，用于定义需要在数据库中生成的表，常用于数据库迁移</br>
生成表内容由 INSTALLED_APPS 应用决定
```
# 在 SQLite 3 中生成表
$ python manage.py migrate
```
sqlite 版本过低需升级</br>
参考：</br>
https://www.cnblogs.com/hszstudypy/p/11512244.html</br>
https://www.cnblogs.com/leffss/p/11555556.html</br>
```
# 报错 sqlite 版本太低
    raise ImproperlyConfigured('SQLite 3.8.3 or later is required (found %s).' % Database.sqlite_versi
django.core.exceptions.ImproperlyConfigured: SQLite 3.8.3 or later is required (found 3.7.17).

# 更新后查看虚拟环境中加载的 sqlite3 版本
(.mysite) [sharonli@vmw-dev-code-01 mysite]$ python
Python 3.6.1 (default, Nov  2 2019, 21:01:57) 
[GCC 4.8.5 20150623 (Red Hat 4.8.5-39)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import sqlite3
>>> sqlite3.sqlite_version
'3.27.2'
>>> 
```
重新生成数据库表
```
$ python manage.py migrate
Operations to perform:
  Apply all migrations: admin, auth, contenttypes, sessions
Running migrations:
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  Applying admin.0001_initial... OK
  Applying admin.0002_logentry_remove_auto_add... OK
  Applying admin.0003_logentry_add_action_flag_choices... OK
  Applying contenttypes.0002_remove_content_type_name... OK
  Applying auth.0002_alter_permission_name_max_length... OK
  Applying auth.0003_alter_user_email_max_length... OK
  Applying auth.0004_alter_user_username_opts... OK
  Applying auth.0005_alter_user_last_login_null... OK
  Applying auth.0006_require_contenttypes_0002... OK
  Applying auth.0007_alter_validators_add_error_messages... OK
  Applying auth.0008_alter_user_username_max_length... OK
  Applying auth.0009_alter_user_last_name_max_length... OK
  Applying auth.0010_alter_group_name_max_length... OK
  Applying auth.0011_update_proxy_permissions... OK
  Applying sessions.0001_initial... OK

```

#### 内置开发服务器
启动 django 内置轻量级开发服务器，django 会动态加载现有代码更新到服务中无需重启</br>
执行 runserver 后，服务器于终端前台启动，默认端口 8000</br>
注：新增文件必须重启服务器，此服务器无法在生产使用
```
$ python manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
February 01, 2020 - 15:31:03
Django version 3.0.2, using settings 'mysite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
[01/Feb/2020 15:33:03] "GET / HTTP/1.1" 200 16351
```
访问虚拟机中 django 服务，需要将虚拟机上的 8000 端口在 nat 上设置映射到外部，参考：https://www.cnblogs.com/coco-shi/p/8689996.html </br>
变更服务器地址为 0.0.0.0 后，外部主机依然无法访问，出现报错
```
$ python manage.py runserver 0.0.0.0:8000
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
February 01, 2020 - 15:39:32
Django version 3.0.2, using settings 'mysite.settings'
Starting development server at http://0.0.0.0:8000/
Quit the server with CONTROL-C.
Invalid HTTP_HOST header: '192.168.45.129:8000'. You may need to add '192.168.45.129' to ALLOWED_HOSTS.
Bad Request: /
[01/Feb/2020 15:39:36] "GET / HTTP/1.1" 400 60169

```
需要将 setting.py 中的主机允许列表改为 *
```
ALLOWED_HOSTS = ["*"]
```

## 创建应用程序
生成应用代码</br>
注意：必须和 manage.py 同级，否则会找不到此模块，需进行额外配置
```
$ python manage.py startapp helloworld
```
应用代码 blog 目录结构
```
.
├── admin.py  # 注册模型
├── apps.py   # 应用配置
├── __init__.py 
├── migrations # 数据库迁移目录
│   └── __init__.py
├── models.py  # 数据模型结构定义
├── tests.py  # 测试代码
├── views.py  # 视图，应用逻辑，一视图对应一 url
└── urls.py  # app 的路由，需自行创建，可在 project urls.py 主路由中导入

1 directory, 7 files
```
编辑应用 views.py
```
 # cat views.py 
from django.shortcuts import render

# Create your views here.

from django.http import HttpResponse

def index(request):
    return HttpResponse("Hello world, Test Sucess!")
```
path() 方法</br>
路由系统 path() 方法，参数 route 及 view 必填、kwargs 和 name 可选</br>

* route: </br>
route 是一个匹配 URL 的准则（类似正则表达式）</br>
当 Django 响应一个请求时，它会从 urlpatterns 的第一项开始，按顺序依次匹配列表中的项，直到找到匹配的项，然后执行该条目映射的视图函数或下级路由（route 不会匹配参数），其后的条目将不再继续匹配，故需注意 urlpatterns 的设置顺序。</br>

* view：</br>
view 为处理当前 url 请求的视图函数</br>
当Django匹配到某个路由条目时，自动将封装的HttpRequest对象作为第一个参数，被“捕获”的参数以关键字参数的形式，传递给该条目指定的视图view。</br>

* kwargs: </br>
任意数量的关键字参数可以作为一个字典传递给目标视图。

* name:</br>
对 url 进行命名
```
# 新建应用 urls.py
# cat urls.py 
from django.urls import path

from . import views

urlpatterns = [
    path('', views.index, name='index'),
]
```
编辑 project urls.py 导入include模块，将 app 的 url 模块添加到文件中</br>
注意：除了admin路由外，尽量给每个app设计自己独立的二级路由
```
# cat urls.py 
"""supervisory_control URL Configuration

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/3.0/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('helloworld/', include('helloworld.urls')),
    path('admin/', admin.site.urls),
]
```
启动开发服务器，访问 127.0.0.1：8000/helloworld 即可

## 启用权限框架管理站点
创建超级用户，启用权限验证框架
```
$ python manage.py createsuperuser
Username (leave blank to use 'sharonli'): admin
Email address: ****@qq.com
Password: 
Password (again): 
Superuser created successfully.
```
访问 http://127.0.0.1:8000/admin 可见登录页面已启用</br>
无论是否有超级用户，这个页面都默认存在
