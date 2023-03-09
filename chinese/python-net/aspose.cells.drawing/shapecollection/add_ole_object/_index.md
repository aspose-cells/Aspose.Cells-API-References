---
title: add_ole_object方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_ole_object/
is_root: false
---
##  add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data) {#int-int-int-int-int-int-bytes}
添加一个 OleObject。


### 返回




```python
def add_ole_object(self, upper_left_row, top, upper_left_column, left, height, width, image_data):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |  |
| top | int |  |
| upper_left_column | int |  |
| left | int |  |
| height | int |  |
| width | int |  |
| image_data | bytes |  |

### 例子

```python
from aspose import pycore

with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    oleObject = shapes.add_ole_object(4, 0, 5, 0, 300, 500, imageData)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
