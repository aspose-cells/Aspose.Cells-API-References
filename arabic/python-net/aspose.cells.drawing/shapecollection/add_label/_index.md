---
title: طريقة add_label
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 130
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف تسمية إلى ورقة العمل.


###  عائدات

كائن تسمية.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ Label من صفه الأيسر ، بوحدة البكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ Label من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع التسمية بوحدة البكسل.|
| width | int | يمثل عرض التسمية بوحدة البكسل.|

###  مثال

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
