---
title: طريقة add_arc
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف شكل قوس إلى ورقة العمل.


###  عائدات

كائن ArcShape.


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ ArcShape من صفه الأيسر ، بوحدة بكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ ArcShape من العمود الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع شكل ArcShape بوحدة البكسل.|
| width | int |يمثل عرض ArcShape بوحدة البكسل.|

###  مثال

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
