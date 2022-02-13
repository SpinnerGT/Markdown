 # 遍历序列对象
- 列表
```jupyter
for x in ["spam","eggs", "ham"]:print(x,end=' ') 
```
- 元组 => [[for循环中运用]]
```jupyter
T =("and","I'm","okay")
for x in T:print(x,end=' ')
```
- 字符串
```jupyter
S = "lumberjack"
for x in S: print(x,end=' ')
```
- 字典()
```jupyter
D={'a':1,b':2,'c':3} 
for key in D: print(key,'=>'D[key]) # 自动获取key

# D.item() 获取(key,value):
for (key,value) in D.items(): 
	print(key,'=>'value)

# 也可以自己手动解包:
for both in D: 
	a,b = both 
```
- 数字  => range




# [[文件]]读取
```jupyter
for line in open('test.txt'): print (line. rstrip)
```
