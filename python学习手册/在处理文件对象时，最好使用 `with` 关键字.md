## 在处理文件对象时，最好使用 `with` 关键字

优点是，子句体结束后，文件会正确关闭，即便触发异常也可以。而且，使用 `with` 相比等效的 [`try`](https://docs.python.org/zh-cn/3/reference/compound_stmts.html#try)-[`finally`](https://docs.python.org/zh-cn/3/reference/compound_stmts.html#finally) 代码块要简短得多：

```python
>>> with open('workfile') as f:
...     read_data = f.read()

>>> # We can check that the file has been automatically closed.
>>> f.closed
True
```
