# vector
## 介绍
vector是向量类型，它可以容纳许多类型的数据，如若干个整数，所以称其为容器，vector是C++STL的一个重要成员。
## 使用
**头文件:**<vector>
**基本操作：**
* vec.push_back(a);尾部插入
* vec[0];下标访问
* 迭代器访问
```c++
    vector<int>::iterator it;
    for(it=vec.begin();it!=vec.end();it++)
        cout<<*it;
```
* vec.insert(vec.begin()+i,a)；在第i+1个元素前面插入a
* vec.erase(vec.begin()+i);删除第i个数
* vec.size();向量大小
* vec.clear();清空
**定义：**vector<Type> vec;
* Type数据类型
## 实现
