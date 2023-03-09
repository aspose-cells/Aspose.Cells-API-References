---
title: intersect方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 110
url: /zh/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
返回一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象，表示两个范围的矩形交集。


### 返回

返回一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象


```python
def intersect(self, range):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| range | [Range](/cells/zh/python-net/aspose.cells/range) |相交范围。|
### 评论

如果两个范围不相交，则返回 null。
### 例子


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A3:A10")
# Get intersected range of the two ranges.
intersectRange = range1.intersect(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
