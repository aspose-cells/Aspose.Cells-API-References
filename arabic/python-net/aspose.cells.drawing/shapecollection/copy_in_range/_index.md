---
title: طريقة copy_in_range
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 380
url: /ar/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
انسخ الأشكال الموجودة في النطاق إلى النطاق الوجهة.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection) | أشكال المصدر.|
| ca | [CellArea](/cells/ar/python-net/aspose.cells/cellarea) | نطاق المصدر.|
| dest_row | int | فهرس صف الإرسال للنطاق المُصْدَر.|
| dest_column | int | عمود الوجهة من نطاق الوجهة.|
| is_contained | bool | ما إذا كان يتم نسخ الأشكال المضمنة في النطاق فقط.<br/> إذا كان صحيحًا ، فقم بنسخ الأشكال الموجودة في النطاق فقط.<br/> خلاف ذلك ، يعمل مثل MS Office.|

###  مثال

```python
from aspose.cells import CellArea

# add a shape
shapes.add_rectangle(2, 0, 2, 0, 130, 130)
area2 = CellArea()
area2.start_column = 1
area2.start_row = 1
area2.end_column = 5
area2.end_row = 11
# copy
shapes.copy_in_range(shapes, area2, 12, 1, False)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
