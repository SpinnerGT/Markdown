# readline()
```jupyter
file = open('test.txt') 
while True: 
	line = file.readline()
	
	if not line:break  # 检测空字符串
	
	print(line.rstrip())
	
```
> 💡每次调用readline方法时，我们就会前进到下一行。当到达文件末尾时，就会返回空字符串，因此我们可通过检测空字符串来跳出循环


# readlines()
readlines()函数一次性把文件载入成每行字符串的*列表*
```jupyter
for line in open('test.txt').readlines(): 
	print(line.rstrip())
```


 类似效果:[[迭代协议]]

 # 翻转文件
 内置函数reversed可以接受一个序列，却不能接受一个生成值的任意可迭代对象
 
 => 换言之，reversed可以接受列表，却不可以接受文件对象

 ```jupyter
for line in reversed(open('test.txt').readlines()):...
```

