---
title: is_gather_string方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
检查单元格的当前字符串值是否需要收集到全局池中。


### 返回

如果需要将字符串值收集到结果文件的全局池中，则为真。


```python
def is_gather_string(self):
    ...
```


### 评论

仅当此实现提供的单元格有许多重复的字符串值时，收集字符串值才会发挥作用。
在这种情况下，收集字符串将节省大量内存并生成更小的结果文件。
如果 LightCellsDataProvider 提供的单元格有很多字符串值，但只有少数相同，
收集字符串将花费更多的内存和时间，并且对生成的文件没有任何优势。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [LightCellsDataProvider](/cells/zh/python-net/aspose.cells/lightcellsdataprovider)
