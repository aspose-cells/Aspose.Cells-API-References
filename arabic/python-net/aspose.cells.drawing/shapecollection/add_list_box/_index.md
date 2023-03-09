---
title: طريقة add_list_box
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 170
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف ListBox إلى ورقة العمل.


###  عائدات

كائن ListBox.


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ ListBox من صفه الأيسر ، بوحدة البكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ ListBox من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع ListBox بوحدة البكسل.|
| width | int | يمثل عرض ListBox بوحدة البكسل.|

###  أمثلة

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
