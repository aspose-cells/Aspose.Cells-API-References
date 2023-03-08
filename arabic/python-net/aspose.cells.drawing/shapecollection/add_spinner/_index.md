---
title: طريقة add_spinner
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 290
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف Spinner إلى ورقة العمل.


###  عائدات

كائن سبينر.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ Spinner من صفه الأيسر ، بوحدة بكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ Spinner من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع Spinner بوحدة البكسل.|
| width | int | يمثل عرض Spinner بوحدة البكسل.|

###  مثال

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
