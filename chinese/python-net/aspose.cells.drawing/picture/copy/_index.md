---
title: copy方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells.drawing/picture/copy/
is_root: false
---
##  copy(source, options) {#Picture-CopyOptions}
复制图片。



```python
def copy(self, source, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source | [Picture](/cells/zh/python-net/aspose.cells.drawing/picture) |图片来源。|
| options | [CopyOptions](/cells/zh/python-net/aspose.cells/copyoptions) |复制选项。|

### 例子

```python
from aspose.cells import CopyOptions, Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
# Copy picture 1 to picture 2.You'll get two picture 1 objects that are superimposed on top of each other.
opt = CopyOptions()
pic2.copy(pic1, opt)
# Save the excel file.
workbook.save("result.xlsx")

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture)
