# 1. 列表
## 1)标志
列表（list），用逗号分隔的不同的数据项用方括号括起来即可。比如：
+ list_sample = [1, 2, 'xiaoli', 'x']
+ 列表索引从0开始，例如：list_sample[2]，打印出 'xiaoli'

## 2)基本操作(创建，append(),pop(),del(),拷贝)
创建方式楼上已述。
+ append()方法表示追加项至列表尾部
  例如：list_sample.append("Zhang san")，打印list_sample，为[1, 2, 'xiaoli', 'x', 'Zhang san']
+ pop()方法表示删除列表的最后一个元素，并将最后一个元素返回
  例如：b = list_sample.pop()，b的值为'Zhang san'，同时list_sample的值变成[1, 2, 'xiaoli', 'x']
+ del方法可以删除指定下标的列表元素，也可以将整个列表进行删除
  例如：del list_sample[2]，之后list_sample变成 [1, 2, 'x']
  例如：del list_sample，再打印list_sample就会报错，因为此时list_sample已经不存在了
+ copy()方法表示拷贝整个列表
  例如：list_sample = [1, 2, 'xiaoli', 'x']
      listCopy = list_sample.copy()
      打印 listCopy得到：[1, 2, 'xiaoli', 'x']
  

## 3)列表相关方法
列表的其他方法还包括
+ remove(x): 删除列表中第一个值为x的元素，若不存在则出错
+ clear(): 删除列表中所有元素。
等等

# 2.元祖
## 1)标志
元组（tuple）是用圆括号包含元素，但是元组的元素不能修改。

## 2)基本操作(创建及不可变性)
+ 创建方法：
  tuple_sample = (1, 2, 'xiaoli', 'x')
+ 如果修改元组的元素，则会报错，例如：

  tuple_sample[0] = 3
  
  '''TypeError                                 Traceback (most recent call last)
<ipython-input-17-dee05ac11933> in <module>()
      1 tuple_sample = (1, 2, 'xiaoli', 'x')
----> 2 tuple_sample[0] = 3

TypeError: 'tuple' object does not support item assignment
'''

# 3.string字符串
## 1)定义及基本操作(+，*，读取方式)
+ 使用单引号或者双引号均可定义字符串，例如：
  s1 = 'abcdefg'
  s2 = "hello world!"
+ "+"加号表示字符串连接，例如：
  s3 = s1 + s2，s3的值为：'abcdefghello world!'
+ "*"星号表示重复输出字符串，例如：
  s4 = s1 * 5，s4的值为：'abcdefgabcdefgabcdefgabcdefgabcdefg'
+ 字符串的读取也可以像列表一样用下标，例如：
  s1[0]，打印出来 'a'

## 2)字符串相关方法
+ find()，用于查询是否包含某子字符串，若查找到返回索引，查不到返回-1
+ count()，返回字符串出现的次数
+ upper()，将字符串中的小写字母全转换为大写字母
+ 。。。


## 4.字符串格式化问题
格式化输出可以用在输出内容部分固定，部分可变的场景，使用"%"操作即可。例如：

name = "起舞"
print("大家好，我叫%s" % name)

打印结果为：大家好，我叫起舞
