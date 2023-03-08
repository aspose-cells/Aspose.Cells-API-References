---
title: طريقة add_radio_button
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 230
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف RadioButton إلى ورقة العمل.


###  عائدات

كائن RadioButton.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ RadioButton من صفه الأيسر بوحدة البكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ RadioButton من عمودها الأيسر ، بوحدة البكسل.|
| height | int |يمثل ارتفاع RadioButton ، بوحدة البكسل.|
| width | int | يمثل عرض RadioButton بوحدة البكسل.|

###  مثال

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
