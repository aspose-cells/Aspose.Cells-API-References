---
title: طريقة add_active_x_control
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
ينشئ عنصر تحكم Activex.


###  عائدات




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | نوع عنصر التحكم.|
| top_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية للشكل من صفه الأيسر ، بوحدة البكسل.|
| left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية للشكل من عمودها الأيسر ، بوحدة البكسل.|
| width | int | يمثل عرض الشكل بوحدات البكسل.|
| height | int | يمثل ارتفاع الشكل بوحدات البكسل.|

###  أمثلة

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
