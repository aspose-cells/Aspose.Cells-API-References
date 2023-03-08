---
title: image_type 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 580
url: /zh/python-net/aspose.cells.drawing/picture/image_type/
is_root: false
---
## image_type 属性

获取图片的图像格式。

### 例子

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
if pic1.image_type == ImageType.PNG:
    pass
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
if pic2.image_type == ImageType.JPEG:
    pass

```
### 定义：
```python
@property
def image_type(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ImageType](/cells/zh/python-net/aspose.cells.drawing/imagetype)
* 类 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture)
