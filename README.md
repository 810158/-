# -
# 1.条件语句
在进行逻辑判断时，我们需要用到条件语句，Python 提供了 if、elif、else 来进行逻辑判断。格式如下所示：
if 判断条件1:
    执行语句1...
elif 判断条件2:
    执行语句2...
elif 判断条件3:
    执行语句3...
else:
    执行语句4...
# 2.循环语句
当需要多次重复执行时，我们要用到循环语句，for 循环和 while 循环。
# 2.1 for循环
for 循环可以遍历任何序列，比如：字符串。如下所示：
str = 'Python'
for s in str:
    print(s)
输出结果：
P
y
t
h
o
n
# 2.2 while循环
while 循环，满足条件时进行循环，不满足条件时退出循环。如下所示：
sum = 0
m = 10
while m > 0:
    sum = sum + m
    m = m - 1
print(sum)
输出结果：
55
# 2.3 break
break 用在 for 循环和 while 循环语句中，用来终止整个循环。如下所示：
str = 'Python'
for s in str:
    if s == 'o':
        break
    print(s)
输出结果：
P
y
t
h
# 2.4 continue
continue 用在 for 循环和 while 循环语句中，用来终止本次循环。如下所示：
str = 'Python'
for s in str:
    if s == 'o':
        continue
    print(s)
输出结果：
P
y
t
h
n
# 3.pass语句
pass 是空语句，它不做任何事情，一般用做占位语句，作用是保持程序结构的完整性。如下所示：
if True:
    pass
    
# 题目
# （1）分数统计if
score=int(input("请输入一个分数\n"))
if 100>=score>=90:
    print('A')
if 90>score>=80:
    print('B')
if 80>score>=60:
    print('C')
if 60>score>=0:
    print('D')
if score<0 or score>100:
    print('错误!')
# （2）分数统计else if
score=int(input("请输入你的分数:\n"))
if 100>=score>=90:
    print('A')
else:
    if 90>score>=80:
        print('B')
    else:
        if 80>score>=60:
            print('C')
        else:
            if 60>score>=0:
                print('D')
            else:
                print('错误!')
# （3）分数统计if elif else
score=int(input("请输入一个分数:\n"))
if 100>=score>=90:
    print('A')
elif 90>score>=80:
    print('B')
elif 80>score>=60:
    print('C')
elif 60>score>=0:
    print('D')
else:
    print('错误!')
