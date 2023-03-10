---
title: طريقة add_scroll_bar
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 250
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---
##  add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
يضيف شريط تمرير إلى ورقة العمل.


###  عائدات

كائن شريط التمرير.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية لـ ScrollBar من صفه الأيسر ، بوحدة بكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | يمثل الإزاحة الأفقية لـ ScrollBar من عمودها الأيسر ، بوحدة بكسل.|
| height | int | يمثل ارتفاع شريط التمرير بوحدة بكسل.|
| width | int | يمثل عرض شريط التمرير بوحدة بكسل.|

###  مثال

```python

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
