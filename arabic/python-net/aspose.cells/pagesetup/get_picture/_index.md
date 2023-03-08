---
title: طريقة get_picture
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 120
url: /ar/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
الحصول على عنصر [Picture](/cells/ar/python-net/aspose.cells.drawing/picture) للرأس / التذييل.


###  عائدات

إرجاع عنصر [Picture](/cells/ar/python-net/aspose.cells.drawing/picture).
العودة فارغة إذا لم يكن هناك صورة.


```python
def get_picture(self, is_header, section):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| is_header | bool | يشير إلى ما إذا كان في الرأس أو التذييل.|
| section | int |0: القسم الأيسر ، 1: القسم الأوسط ، 2: القسم الأيمن.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
الحصول على عنصر [Picture](/cells/ar/python-net/aspose.cells.drawing/picture) للرأس / التذييل.


###  عائدات

إرجاع عنصر [Picture](/cells/ar/python-net/aspose.cells.drawing/picture).


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| is_first | bool | يشير إلى ما إذا كان يتم الحصول على صورة رأس / تذييل الصفحة الأولى.|
| is_even | bool | يشير إلى ما إذا كان يتم الحصول على صورة رأس / تذييل الصفحة الزوجية.|
| is_header | bool |يشير إلى ما إذا كان يتم الحصول على صورة الرأس / التذييل.|
| section | int |0: القسم الأيسر ، 1: القسم الأوسط ، 2: القسم الأيمن.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PageSetup](/cells/ar/python-net/aspose.cells/pagesetup)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)
