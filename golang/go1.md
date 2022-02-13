---
tag: go
aliases:
---

`package main`:如果要直接（通常从终端）运行此代码，这个是必需的

`func main()`:一个Go程序运行时，它会寻找一个名为main的函数并首先运行它，这就是为什么我们将这个函数命名为main

go文件布局(典型)：
![[Pasted image 20220121141818.png]]

分号不是必须滴!

`go fmt` 格式化工具

---
函数:

	使用参数向函数提供数据

调用函数:`包名.函数名`

返回值:

	程序需要能够调用函数并从那儿获取数据。因此，大多数编程语言中的函数都可以有返回值：函数计算后并返回给调用者的值

符文rune:单个字符
> 因为Go使用Unicode标准来存储rune。rune被保存为数字代码，而不是字符本身


可以使用小数点来区分整数和浮点数


类型:指定了用途

	交通工具只能用来坐而不能用来吃
	食物只能吃而不能用来坐

Go是静态类型的，这意味着它甚至在程序运行之前就知道值的类型是什么
> 查看类型:`reflect`包下的`TypeOf`函数:
> `reflect.TypeOf()`


---

变量: 包含值的一块存储

> 要先声明才能赋值

1.先声明后赋值
```
var 变量名 变量类型   //声明变量
变量名 = 值    //赋值

变量名1,变量名2...=值1,值2... //可以在同一语句中为多个变量赋值
```

2.事先知道变量的值是什么
```go

var 变量名 变量类型 = 值 //复杂

var 变量名 = 值 //稍微简单

变量名 := 值  //短变量声明
```


```ad-note
如果声明一个变量而没有给它赋值，该变量将包含其类型的零值:
- int/float = 0
- string = ''
- bool = false
```


注意:

| 同一变量只能一次声明 | 声明变量必须使用 |
| -------------------- | ---------------- |

---


命名规则:

	
	- 大写-包外可以访问
	- 小写-只能包内
	
	- 驼峰命名



类型转换:

	1.任何数学运算中，或者与其他float64值进行比较前，先将int值转换为float64值



电脑运行:

	1.切换到目录
	2.go build xx.go   
	//生成二进制执行文件,即使对方没有go环境也可以运行
	
	3.`./xxx`运行


快速运行:

	go run xx.go

---

