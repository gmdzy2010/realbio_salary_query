=====
realbio-salary-query
=====

realbio-salary-query 为给公司行政部门增加的工资查看功能所做的可复用Django app。现在为初始版本

如何使用
-----------

1. 将 "realbio_salary_query" 添加到你的项目settings.py的 INSTALLED_APPS 中::

    INSTALLED_APPS = [
        ...
        'realbio_salary_query',
    ]

2. 将django-salary-query的url添加你的项目总url当中::

    url(r'^salary_query/', include('realbio_salary_query.urls')),

3. 运行`python manage.py migrate`构建realbio_salary_query的数据库表.

4. 运行django的开发服务器，访问 http://127.0.0.1:8000/admin/.

5. 登陆用户界面即可查询自己的工资.
