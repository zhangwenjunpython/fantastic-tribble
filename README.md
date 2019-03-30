##存贮考试一些代码

#第一行为获取时间
#%b	月份名称缩写	Jan~Dec，例如：Apr
#%A	星期	Monday~Sunday，例如：Wednesday
# %a	星期缩写	Mon~Sun，例如：Wed
# %H	小时（24h制）	00~23，例如：12
# %h	小时（12h制）	01~12，例如：7
# %p	上/下午	AM, PM，例如：PM
# t = time.gmtime()
# print(time.strftime("%Y-%m-%d %H:%M:%S",t))


#------------------------------------------------
# 保留两位小数输出
# print("{:.2f}".format(f(n)))

#-----------------------------------------------
# from turtle import * 引入turtle库的所有函数 (引入之后可以不用写t.函数)
# from turtle import *  
# fillcolor("red")
# circle(10,360)
# turtle.end_fill()


#--------------------------------------------------
#中文分词jieba处理
# import jieba
# txt = open("阿甘正传-网络版.txt","r",encoding ="utf-8")
# words = jieba.lcut(txt)

#统计某个词的数量：先定义counts={} get获得某个键对应的值，如果某有还回0
#counts[word] = counts.get(word,0)+1

# items = list(counts.items())          #items还回字典所有的键值对，生成元组，list把元组都合并成一个列表
# sort是原地排序，x:x[1]是对列表中每个小列表序号为1的元素为依据排列每个小元素   （注意sorted不是原地操作，还回一个列表值）
# 其中reverse=Ture是从大到小排序
# items.sort(key = lambda x:x[1],reverse = True)

#分别读取列表中的每个小元素
# for i in range(10):
#   word,count = items[i]

#replace是替换函数，这个不是原地操作，所有要赋值给一个变量。前面是old 后面是new，记得双引号
# line = line.replace("\n","")
# ls.append(line)  

#Python 字典(Dictionary) keys() 函数以列表返回一个字典所有的键。
#for key in fruits.keys():
#values() 函数以列表返回字典中的所有值，跟keys一样还回一个列表

#pip install -U pip

# import random
# k = random.uniform(10,100)   #不包括100

##冒泡排序法
# for i in range(n):
#         for j in range(i, n)
#             if lst[i] <lst[j]:
#                 lst[i],lst[j]=lst[j],lst[i]    

#切片和输出
#lst = numbers.split(',')      切片不是原地操作，要赋值出去
#print(','.join(slst))         把列表按某个连接符号给连接起来输出

# strip() 方法用于移除字符串头尾指定的字符（默认为空格或换行符）或字符序列。（默认不写的话就是把回车换行之类的去掉
#用法是  str.strip（"内容"），不会原地操作所以要赋值出去

# line = "abcde"
# line[:-1]              #0到-1不包括-1
# 结果为：'abcd'
# line = "abcde"
# line[::-1]
# 结果为：'edcba'

# fieds.append(fi)    #原地操作

#  ls1.pop(x)  原地操作，直接删除字典的某个键值对

#  num,count = items[0]    快速对列表中的赋值

#print(line.center(30,chr(12288)))    center是居中处理 30是长度，chr是插入的东西，还回更新后的列表
# L.insert(2,*)        在2这个位置插入*，没有还回值，是原地操作

# for k,v in dic.items():    键值对依次赋值到k，v   

# ones = i % 10                 个十百位数
#tens = i // 10 % 10
#hundreds = i // 100


#---------------------------------
# m = input("")
# s = "PYTHON"
# if  m =="右":
#     m = ">"
# elif  m =="中":
#     m = "^"
# else:
#     m = "<"
# print("{0:*{1}30}".format(s, m))
