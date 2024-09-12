# 1 base
### 1.1 常用字符串内建函数
- 首字母大写（capitalize）
- 以字串结尾（endswith）、以字串开头（startswith）
- 是否是数字（isdigit）
- 小写化（lower）
- 去掉两端的空白字符（strip）
- 替换（replace）
- 合并（join）
- 字符串长度
[detail string knowledge](https://www.runoob.com/python3/python3-string.html)

### 1.2 列表常见的编辑操作
- 追加元素到尾部（append）
- 插入元素到固定位置（insert）
- 删除特定位置元素（remove）
- 弹出尾部元素（pop）
- 合并两个列表（extend）
- 反转（reverse）
- 排序（sort）
  
 #### extend和“+”的区别
 - extend改变的是第一个列表，原地操作
 - 拼接“+”，原始列表不变，返回一个新的列表

# 2 正则
[regex01.com](regex101.com)和[c.runoob.com](c.runoob.com)可以测试正则
描述|正则|测试字符串
--|--|--
身份证|^(\d{15} \| \d{18})$|123454

# 3 文件
文件打开模式
•"r" 只读模式，如文件不存在，报错
•“w” 覆盖写模式，如文件不存在，则创建；如文件存在，则完全覆盖原文件
•“x” 创建写模式，如文件不存在，则创建；如文件存在，报错
•"a” 追加写模式，如文件不存在，则创建；如文件存在，则在原文件后追加内容
•“b” 二进制文件模式，不能单独使用，需要配合使用如”rb”，“Wb”，“ab"，该模式不需指定encoding
•“+”，与"w", ”x”，"a"配合使用，在原功能基础上，增加读写功能
•打开模式缺省，默认为只读模式
