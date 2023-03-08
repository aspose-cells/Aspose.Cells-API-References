---
title: طريقة add_line
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 150
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف LineShape إلى ورقة العمل.


###  عائدات

كائن LineShape.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ LineShape من صفه الأيسر ، بوحدة البكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ LineShape من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع LineShape بوحدة البكسل.|
| width | int | يمثل عرض LineShape بوحدة البكسل.|

###  مثال

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
