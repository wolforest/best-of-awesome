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
In : a = 1
In : b = 1
In : id(a)
Out: 140708412432784
In : id(b)
Out: 140708412432784
In : a is b
Out: True

In : s1 = 'abc'
In : s2 = 'abc'
In : id(s1)
Out: 1554773534064
In : id(s2)
Out: 1554773534064
In : s1 is s2
Out: True
```
```
#string
In : '234' in '12345'
Out: True

#list
In : [1,2] in [[1,2],3,'abc']
Out: True
In : lst = [[1,2],3,'abc']
In : [1,2] in lst
Out: True
In : 'abc' in lst
Out: True

#dict
In : dct = {'a':12,'b':35,'key':'abc'}
In : 'a' in dct
Out: True
In : 'key' in dct
Out: True

In : 12 in dct
Out: False
In : 12 in dct.values()
Out: True
In : 'abc' in dct.values()
Out: True
```


