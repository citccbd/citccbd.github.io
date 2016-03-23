---
layout: post
title: "解决Service Monitor内部错误的问题"  
date: 2016-03-09 15:26:13  
categories: Hadoop，     CDH
---
## **问题描述：** 
CDH集群运行一段时间后，经常会出现Service Monitor内部错误的问题，导致无法有效监控集群状态

如下图所示：


![](http://i.imgur.com/Pnml8NG.jpg)  




## **解决方案：**

### **1. 重启cloudera-scm-service服务** 


- ### 执行命令： 
   
             
             service cloudera-scm-server restart 
   
   

- ### 查询server状态：

             service  cloudera-scm-server status
  

### **2. web界面重启Service Monitor：** 

如下图所示：

![](http://i.imgur.com/AvNeXuc.jpg)


### **3. 问题原因** ##
   初步猜测是由于服务器系统性能不足导致，尚不确定



