---
title: طريقة add_text_box
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 310
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف مربع نص إلى ورقة العمل.


###  عائدات

عنصر [TextBox](/cells/ar/python-net/aspose.cells.drawing/textbox).


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int |يمثل الإزاحة الرأسية لمربع النص من صفه الأيسر ، بوحدة بكسل.|
| upper_left_column | int |فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لمربع النص من العمود الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع مربع النص ، بوحدة البكسل.|
| width | int | يمثل عرض مربع النص بوحدة البكسل.|

###  مثال

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
* فئة [TextBox](/cells/ar/python-net/aspose.cells.drawing/textbox)
