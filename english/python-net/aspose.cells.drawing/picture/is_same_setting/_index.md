---
title: is_same_setting method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 140
url: /python-net/aspose.cells.drawing/picture/is_same_setting/
is_root: false
---

## is_same_setting(obj) {#any}

Returns whether the shape is same.


### Returns 





```python
def is_same_setting(self, obj):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| obj | any |  |

### Example 


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



### See Also
* module [aspose.cells.drawing](../../)
* class [Picture](/cells/python-net/aspose.cells.drawing/picture)
