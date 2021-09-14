# map
## 介绍
map以模板(泛型)方式实现，可以存储任意类型的数据，包括使用者自定义的数据类型。Map主要用于资料一对一映射(one-to-one)的情況，map內部的实现自建一颗红黑树，这颗树具有对数据自动排序的功能。在map内部所有的数据都是有序的
## 使用
**头文件:**<map>
**基本操作：**
* mymap.insert(pair<int,int>(0,1));插入
* mymap.insert(map<int,int>::value_type(0,1));插入
* mymap[0]=1;插入
* iter = mymap.find("123");查找，找到返回所在位置，否则返回mymap::end()
* mymap.erase(iter);删除
* mymap.clear();清空==mymap.erase(mymap.begin(),mymap.end());
* mymap.size();返回大小
**定义：**map<Type, Type> mymap;
* Type数据类型
## 实现
