# Cuf

简单做了个可视化系统

index 页面：钢铁生产流程

技术展示页面：可以选中技术并绘制条形图、潜力饼图、成本散点图

数据仪表盘页面：展示各个流程用到的技术

流程分析：主要有三个图表。条形图  热力图  玫瑰图。

由于直接把技术名称放在表上会造成严重的数据重叠，因此在旁边写了个编号——名称的table

可能需要做修改的地方：

1. 图表的颜色
2. 图表上数字的大小
3. 图表布局


使用说明：

1. 电脑需要安装python
2. 下载源码后，切换到与manage.py同级的目录
3. 创建虚拟环境（命令是 python -m venv myenv）
4. 激活虚拟环境（命令是 myenv\Scripts\activate）  （实际上是找到虚拟环境名的文件夹下的Scripts\activate，激活虚拟环境）
4. 安装需求的包（命令是 pip install -r requirements.txt）
5. 配置数据文件
   1. 在与manage.py同级的目录下创建文件夹paper
   2. 在文件夹paper下放入数据 data.xlsx
   3. 或者选择进入settings文件夹下的__init__.py 修改 DATA_FILE_NAME 和 DATA_FILE_PATH 两个参数
6. 进入虚拟环境后，切换到与manage.py同级的目录，在终端输入命令 python manage.py
7. 程序运行成功后在终端会出现以下信息，输入Running on 的网址即可打开页面。或者按住ctrl后单击网址，可直接打开页面。

* Serving Flask app 'apps'
* Debug mode: on
  WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
* Running on http://127.0.0.1:5000
  Press CTRL+C to quit
* Restarting with stat
* Debugger is active!
* Debugger PIN: 404-367-758
