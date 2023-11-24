conda create -n django4 python=3.11.5
conda activate django4
conda clean --index-cache
conda update pip
pip install django -i https://mirrors.aliyun.com/pypi/simple/
(使用第一种成功，以下是官方安装，可能出错）
python -m pip install Django
查看django版本：
$ python -m django --version
>>> import django
>>> print(django.get_version())
4.2.7

安装完django pip列表如下：
(django4) PS D:\> pip list
Package    Version
---------- -------
asgiref    3.7.2
Django     4.2.7
pip        23.3.1
setuptools 68.0.0
sqlparse   0.4.4
tzdata     2023.3
wheel      0.41.2

中文官方：
https://docs.djangoproject.com/zh-hans/4.2/
https://docs.djangoproject.com/zh-hans/4.2/intro/tutorial01/
https://www.bookstack.cn/read/Django-4.0-zh/fe6cf677b8556466.md


django-admin startproject mysite
cd mysite
python manage.py runserver

python manage.py runserver 8080

python manage.py startapp polls

python manage.py migrate


git remote add origin https://github.com/j4go/mysite.git
git branch -M main
git push -u origin main