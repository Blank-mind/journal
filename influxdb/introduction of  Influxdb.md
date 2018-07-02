#  Influxdb 入门

### 本文内容

本文将介绍Influxdb的基本概念，基本操作，一些demo实践，本文不会介绍Influxdb的安装配置，Influxdb与其他数据库的比较以及过多的废话。

### 什么是Influxdb？

简单的说，Influxdb是一个时间序列数据库。时间序列数据库主要用来存储时间序列数据，而时间序列数据简单地说就是带有时间戳的数据。

### Influxdb的基本概念

+ database
  类似于传统关系型数据库中的database的概念。

+ measurement
     类似于传统关系型数据库中的tablede概念。

+ point
     point主要由时间戳（time),数据（field),标签（tags)组成。
     - time 
       每个数据记录时间，会默认生成，值为当地时间，同时也是数据的索引。

     - field
       各种记录值，不带有索引，用二维图表来理解的话一般是图表的纵坐标。

     - tags
       各种带有索引的属性，用二维图表来理解的话一般是图表的横坐标。

+ series

     数据库里的数据，都需要通过图表来展示，而series就表示这个表里面的数据可以用几条线画出来，可以通过tag的排列组合算出来。

### Influxdb的基本操作

+ 操作方式

  - 命令行交互

  - HTTP 

  - 第三方语言API

+ 基本常见操作

  - 指定使用某个数据库，如mydb
    ```
    use mydb
    ```
  - 查看所有数据库
 	```
 	show databases
 	```




    

  

  

  







