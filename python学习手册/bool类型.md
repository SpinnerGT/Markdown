
# bool与int
boo1实际上只是内置整数类型int的子类（从面向对象的角度来看） => True和Fa1se的行为与整数1 和0是一样的

只不过它们有独特的显示逻辑：它们是作为关键字True和False显示的， 而不是数字1和0。

> bool为这两个对象重新定义了str和repr的字符串格式