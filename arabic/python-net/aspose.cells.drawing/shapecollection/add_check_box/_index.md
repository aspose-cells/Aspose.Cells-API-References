---
title: طريقة add_check_box
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف مربع اختيار إلى ورقة العمل.


###  عائدات

فهرس كائن CheckBox الجديد.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int |يمثل الإزاحة الرأسية لخانة الاختيار من صفها الأيسر ، بوحدة البكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لمربع النص من العمود الأيسر ، بوحدة البكسل.|
| height | int | ارتفاع مربع النص ، بوحدة البكسل.|
| width | int | عرض مربع النص ، بوحدة البكسل.|

###  أمثلة

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
