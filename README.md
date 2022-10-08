## 零、项目获取

获取方式（点击下载）：[是云猿实战](http://shiyuncode.com/details?id=44)
项目经过多人测试运行，可以确保100%成功运行。

## 一、项目简介

本系统结合众多公安警情案例以及各方面综合信息，再通过WEB技术进行可视化分析以及管理，多维度的观察分析这些数据，也有利于公安系统做出一些相关的决策。

本系统Python Web技术为基础，Flask为开发的WEB框架，以MySQL为数据库，展开对公安警情系统可视化的详细分析与研究。

## 二、开发环境

运行环境：推荐Python3.6及以上；

开发工具：PyChram（推荐）；

操作系统：windows 10 8G内存以上（其他windows以及macOS支持，但不推荐）；

浏览器：Firefox(推荐)、Google Chrome(推荐)、Edge;

数据库：MySQL8.0(推荐)及其他版本（支持但不推荐，尤其MySQL5.6及以下）；

数据库可视化工具：Navicat Premium 15（推荐）以及其他Navicat版本

## 三、项目技术

后端：Flask、PyMySql

前端：HTML、Jquery、Ajax、LayUI、Echarts

## 四、功能结构

普通用户模块有可视化模块、公告查看功能、版本查看功能。

 

针对管理员权限的功能模块包括可视化模块，用户管理功能、公告管理功能，版本管理功能、警情类别管理功能、警情性质管理功能、以及警情管理功能。

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)

## 五、运行截图

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image006.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image006.png)

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image010.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image012.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image014.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image016.png)

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image018.png)

 

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image020.png)

![img](file:///C:/Users/胡云飞/AppData/Local/Temp/msohtmlclip1/01/clip_image022.jpg)

 

## 六、数据库设计

case表

| **字段名称** | **数据类型**  | **是否必填** | **注释** |
| ------------ | ------------- | ------------ | -------- |
| **id**       | int           | 是           | 主键     |
| **price**    | decimal(10,2) | 否           | 损失价格 |
| **sex**      | varchar(2)    | 否           | 性别     |
| ...          | ...           | ...          | ...      |
| ...          | ...           | ...          | ...      |
| ...          | ...           | ...          | ...      |
| ...          | ...           | ...          | ...      |
| ...          | ...           | ...          | ...      |
| **rep_time** | datetime      | 否           | 报案时间 |

 

category表

| **字段名称** | **数据类型** | **是否必填** | **注释** |
| ------------ | ------------ | ------------ | -------- |
| **id**       | int          | 是           |          |
| **content**  | varchar(255) | 否           | 类型     |

 

notice表

| **字段名称**    | **数据类型** | **是否必填** | **注释** |
| --------------- | ------------ | ------------ | -------- |
| **id**          | int          | 是           | 公告     |
| **title**       | varchar(255) | 否           | 公告标题 |
| **content**     | varchar(255) | 否           | 公告内容 |
| **user_name**   | varchar(255) | 否           | 发布人   |
| **create_time** | datetime     | 否           | 发布时间 |

 

sys_version表

| **字段名称**    | **数据类型** | **是否必填** | **注释** |
| --------------- | ------------ | ------------ | -------- |
| **id**          | int          | 是           | 系统版本 |
| **sys_name**    | varchar(255) | 否           | 名称     |
| **sys_version** | varchar(255) | 否           | 描述     |

 

type表

| **字段名称** | **数据类型** | **是否必填** | **注释** |
| ------------ | ------------ | ------------ | -------- |
| **id**       | int          | 是           |          |
| **content**  | varchar(255) | 否           | 类型     |

 