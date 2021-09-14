# unordered_map
## 介绍
unordered_map和map类似，都是存储的key-value的值，可以通过key快速索引到value。不同的是unordered_map不会根据key的大小进行排序，存储时是根据key的hash值判断元素是否相同，即unordered_map内部元素是无序的。
## 使用
**头文件:**<map>
**基本操作：**
* mymap.insert(pair<int,int>(0,1));插入
* mymap.insert(unordered_map<int,int>::value_type(0,1));插入
* mymap[0]=1;插入
* iter = mymap.find("123");查找，找到返回所在位置，否则返回mymap::end()
* mymap.erase(iter);删除
* mymap.clear();清空==mymap.erase(mymap.begin(),mymap.end());
* mymap.size();返回大小
**定义：**unordered_map<Type, Type> mymap;
* Type数据类型
## 实现
