---
title: original_height_cm 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 930
url: /zh/python-net/aspose.cells.drawing/picture/original_height_cm/
is_root: false
---
## original_height_cm 属性

获取图片的原始高度，单位为厘米。

### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original height of the picture.
picHeightCM = pic.original_height_cm
# Save the excel file.
workbook.save("result.xlsx")

```
### 定义：
```python
@property
def original_height_cm(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture)
