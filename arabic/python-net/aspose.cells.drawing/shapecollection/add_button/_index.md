---
title: طريقة add_button
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 60
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف زرًا إلى ورقة العمل.


###  عائدات

كائن زر.


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ Button من صفه الأيسر ، بوحدة بكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ Button من عمودها الأيسر ، بوحدة بكسل.|
| height | int | يمثل ارتفاع الزر ، بوحدة البكسل.|
| width | int | يمثل عرض الزر ، بوحدة البكسل.|

###  أمثلة

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
