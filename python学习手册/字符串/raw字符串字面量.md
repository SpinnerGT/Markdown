# 原始字符串阻止转义

通常出现在windows路径上,为了修复这样的文件名错误，记得在Windows系统上增加字母r:
```jupyter
myfile =  open(r'C:\new\text.dat','w')
```

或者[[反斜线转义字符#双|双\\]]

