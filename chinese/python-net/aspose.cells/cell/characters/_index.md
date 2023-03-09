---
title: characters方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
返回一个 Characters 对象，该对象表示单元格文本中的 characters 范围。


### 返回

字符对象。


```python
def characters(self, start_index, length):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| start_index | int |字符开始的索引。|
| length | int |字符数。|
### 评论

此方法仅适用于具有字符串值的单元格。
### 例子


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
