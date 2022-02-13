`f.read(size)` 可用于读取文件内容，它会读取一些数据，并返回字符串（文本模式），或字节串对象（在二进制模式下)

如已到达文件末尾，`f.read()` 返回空字符串（`''`）


# 一次加载至字符串
# 每个字符加载
```jupyter
file = open('test.txt') 

while True: 
	char file.read(1)  # Read by character
	if not char:break  # Empty string means end-of-file
	print(char) 
	
for char in open('test.txt').read():
	print(char)
```
> 💡 按字符读取的文件末尾识别


# bytes(块)为单位加载

> 通常会按块读取**二进制数据**
```jupyter
file = open('test.txt','rb') 
while True: 
	chunk file.read(10)  # Read byte chunks:up to 10 bytes
	if not chunk:break 
	print(chunk)
```