---
title: is_same_setting方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 140
url: /zh/python-net/aspose.cells.drawing/picture/is_same_setting/
is_root: false
---
##  is_same_setting(obj) {#any}
返回形状是否相同。


### 返回




```python
def is_same_setting(self, obj):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| obj | any |  |

### 例子

```python
from aspose.cells import Workbook

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
if pic1.is_same_setting(pic1):
    pass
if !pic1.is_same_setting(pic2):
    pass

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture)
