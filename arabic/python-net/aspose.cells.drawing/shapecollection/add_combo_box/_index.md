---
title: طريقة add_combo_box
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 80
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_combo_box/
is_root: false
---
##  add_combo_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف ComboBox إلى ورقة العمل.


###  عائدات

كائن ComboBox.


```python
def add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ ComboBox من صفه الأيسر بوحدة البكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ ComboBox من عمودها الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع ComboBox بوحدة البكسل.|
| width | int | يمثل عرض ComboBox بوحدة البكسل.|

###  مثال

```python

# add a combo box
comboBox = shapes.add_combo_box(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
