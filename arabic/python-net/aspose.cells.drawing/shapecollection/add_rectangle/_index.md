---
title: طريقة add_rectangle
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 240
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف RectangleShape إلى ورقة العمل.


###  عائدات

كائن RectangleShape.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ RectangleShape من صفه الأيسر بوحدة البكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ RectangleShape من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع RectangleShape بوحدة البكسل.|
| width | int | يمثل عرض RectangleShape بوحدة البكسل.|

###  مثال

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
