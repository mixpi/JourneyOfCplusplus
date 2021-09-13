# priority_queue
## 介绍
在优先队列中，元素被赋予优先级。当访问元素时，具有最高优先级的元素最先删除，最高优先级先出的行为特征。优先队列具有队列的所有特性，包括队列的基本操作，只是在这个基础上添加了内部的一个排序，本质是一个堆实现的。
## 使用
**头文件:**<queue>
**基本操作：**
* top访问对头元素
* empty队列是否为空
* size返回队列内元素个数
* push插入元素到队列（并排序）
* emplace 原地构造一个元素并插入队列
* pop弹出队头元素
* swap交换内容
**定义：**priority_queue<Type, Container, Functional> pq;
* Type数据类型
* Container容器类型(必须是数组实现的容器，默认是vector)
* Functional比较方式
```c++
    //升序队列，小顶堆，一定要有空格
    priority_queue<int, vector<int>, greater<int> > q;
    //降序队列，大顶堆，默认
    priority_queue<int, vector<int>, less<int> > q;
```
## 实现
