---
title: auto_fill方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/range/auto_fill/
is_root: false
---
##  auto_fill(target) {#Range}
自动填充目标范围。



```python
def auto_fill(self, target):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| target | [Range](/cells/zh/python-net/aspose.cells/range) |目标范围。|

### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
source = cells.create_range("A1:A2")
target = cells.create_range("A3:A10")
# fill 3,4,5....10 to the range A3:A10
source.auto_fill(target)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  auto_fill(target, auto_fill_type) {#Range-AutoFillType}
自动填充目标范围。



```python
def auto_fill(self, target, auto_fill_type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| target | [Range](/cells/zh/python-net/aspose.cells/range) |目标范围。|
| auto_fill_type | [AutoFillType](/cells/zh/python-net/aspose.cells/autofilltype) |自动填充类型。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
