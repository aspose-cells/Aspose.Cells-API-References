---
title: add_free_floating_shape方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
向工作表添加自由浮动形状。仅适用于线条/图像形状。


### 返回




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/zh/python-net/aspose.cells.drawing/msodrawingtype) |形状类型。|
| top | int |表示形状相对于工作表顶行的垂直偏移量，以像素为单位。|
| left | int |表示形状相对于工作表左列的水平偏移量，以像素为单位。|
| height | int |表示 LineShape 的高度，以像素为单位。|
| width | int |表示 LineShape 的宽度，以像素为单位。|
| image_data | bytes |图片资料，只适用于图片。|
| is_original_size | bool |如果形状是图像，形状是否使用原始大小。|

### 例子

```python
from aspose import pycore
from aspose.cells.drawing import MsoDrawingType

# add a line
floatingShape_Line = shapes.add_free_floating_shape(MsoDrawingType.LINE, 100, 100, 100, 50, None, False)
# add a picture
imageData = None
with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
floatingShape_Picture = shapes.add_free_floating_shape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, False)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
