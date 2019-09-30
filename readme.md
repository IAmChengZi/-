# 缓冲区溢出：原理与实验

### 哈尔滨工业大学 网络与信息安全 2016-2018

### 姓名：程蕾蓉      
### 学号：19S003101

---

### 实验一
#### 漏洞一：strcat函数
1.利用grep来查找所有.c文件中的strcat函数，发现在http.c文件中有三处调用了strcat函数。

2.分别定位到http.c中的对应位置，浏览该处的包含strcat的函数代码。


3.分析http_serve()函数中对strcat函数的调用，发现strcat(pn,name)中pn数组的大小为1024且name变量来自于http_serve()的传入参数const char *name,因此有利用grep来查找调用过http_serve()的函数，发现在zookfs.c文件中调用了。

4.定位到zookfs.c中的对应位置，经分析后发现

#### 漏洞二：函数
### 实验二

