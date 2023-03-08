---
title: delete_in_range方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 400
url: /zh/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
删除范围内的形状。注释形状不会被删除。



```python
def delete_in_range(self, ca):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| ca | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |范围。如果形状包含在范围内，它们将被删除。|

### 例子

```python
from aspose.cells import CellArea

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
area3 = CellArea()
area3.start_column = 0
area3.start_row = 5
area3.end_column = 5
area3.end_row = 8
# del
shapes.delete_in_range(area3)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
