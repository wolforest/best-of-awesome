# python basic syntax - for experienced programmer

### None
The None keyword is used to define a null value, or no value at all.
None is not the same as 0, False, or an empty string. None is a data type of its own (NoneType) and only None can be None.

### 万能的not
```
not None == not False == not '' == not 0 == not [] == not {} == not ()
```

### is in ==
is 用于判断两个变量引用对象是否为同一个
== 用于判断引用变量的值是否相等
in 用于成员检测

Python 中使用 id() 函数获取对象的标识号，可以理解为内存地址
```
In [49]: a = 1
In [50]: b = 1
In [51]: id(a)
Out[51]: 140708412432784
In [52]: id(b)
Out[52]: 140708412432784
In [53]: a is b
Out[53]: True

In [54]: s1 = 'abc'
In [55]: s2 = 'abc'
In [56]: id(s1)
Out[56]: 1554773534064
In [57]: id(s2)
Out[57]: 1554773534064
In [58]: s1 is s2
Out[58]: True
```
```
#string
In [104]: '234' in '12345'
Out[104]: True

#list
In [106]: [1,2] in [[1,2],3,'abc']
Out[106]: True
In [107]: lst = [[1,2],3,'abc']
In [109]: [1,2] in lst
Out[109]: True
In [110]: 'abc' in lst
Out[110]: True

#dict
In [111]: dct = {'a':12,'b':35,'key':'abc'}
In [112]: 'a' in dct
Out[112]: True
In [113]: 'key' in dct
Out[113]: True

In [114]: 12 in dct
Out[114]: False
In [115]: 12 in dct.values()
Out[115]: True
In [116]: 'abc' in dct.values()
Out[116]: True
```


