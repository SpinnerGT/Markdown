---
tag: python/核心对象/文件/print
aliases:
---


- 文件对象方法
文件写人方法是把字符串写入到任意的文件中,而print则是默i人地把对象写人stdout流


- stdout标准输出流
标准输出流通常映射到Python程序的启动窗口

> 复杂的字符串使用格式化:
> ![[Pasted image 20220129144447.png]]


# 语法

```python
print(ob1,ob2,sep='',end='\n',file=sys.stdout)
```


## file
定向输出到一个文件
![[Pasted image 20220129144422.png]]


# print的等价操作
![[Pasted image 20220129144722.png]]
![[Pasted image 20220129152320.png]]

## 使用

把sys.stdout重新赋值给标准输出流以外的对象。
换句话说，这提供了一种可以让print语句将文字发送到其他地方的等效方式
![[Pasted image 20220129144915.png]]

> 切换回来: [[tmp暂存sys.stdout]]

- 一次性使用: file重定向
![[Pasted image 20220129145951.png]]



