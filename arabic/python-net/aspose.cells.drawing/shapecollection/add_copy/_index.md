---
title: طريقة add_copy
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 90
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
يضيف شكلاً ونسخه إلى ورقة العمل.


###  عائدات

فهرس كائن الشكل الجديد.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_shape | [Shape](/cells/ar/python-net/aspose.cells.drawing/shape) | شكل المصدر.|
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int |يمثل الإزاحة الرأسية لخانة الاختيار من صفها الأيسر ، بوحدة البكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لمربع النص من العمود الأيسر ، بوحدة البكسل.|

###  مثال

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
