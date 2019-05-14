# Dict字典

## 定义
+ 字典包含很多键值对，用花括号包裹。每个键值对用冒号：分割，每对之间用逗号，分割

## 创建
+ dict1 = {'a': 1, 'b': 2, 'c': 3}

## 字典的方法
包括keys、values、items、clear等方法。
+ dict1.keys(), 输出：dict_keys(['a', 'b', 'c'])
+ dict1.values(), 输出：dict_values([1, 2, 3])
+ dict1.items(), 输出：dict_items([('a', 1), ('b', 2), ('c', 3)])
+ dict1.clear(), 无输出，但是dict1已被清空


# 集合

## 特性
+ 用花括号定义，元素不重复，无序，因此不记录元素位置或插入点，不支持索引、切片等操作。只有键没有值

## 创建
+ s1 = {1, 2, 3, 4, 5}

## 方法
方法有add, update, pop, remove, clear等
+ s1.add(3.5), 打印s1为：{1, 2, 3, 3.5, 4, 5}
+ s1.update({2, 4, 6, 8}),打印s1为：{1, 2, 3, 3.5, 4, 5, 6, 8}
+ s1.pop(), 返回值为：1
+ s1.remove(3), 打印s1为： {2, 3.5, 4, 5, 6, 8}
+ s1.clear(), 无返回值，s1已清空


# 判断语句（要求掌握多条件判断）
+ 语法是：
  if 条件1：
    语句块1
  elif 条件2：
    语句块2
  else:
    语句块3
    

# 三目表达式
+ 输入两个数，比较它们的大小并输出其中较大者
+ print(x if(x>y) else y)
例如：
  x = input()
  y = input()
  print(x if(x>y) else y)


# 循环语句
+ for i in range(5):
    print(i)
+ 打印结果：
0
1
2
3
4
