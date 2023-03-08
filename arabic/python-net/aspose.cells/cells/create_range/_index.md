---
title: طريقة create_range
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 190
url: /ar/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
لتكوين عنصر [Range](/cells/ar/python-net/aspose.cells/range) من عنوان النطاق.


###  عائدات

عنصر [Range](/cells/ar/python-net/aspose.cells/range)


```python
def create_range(self, address):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| address | str | عنوان النطاق.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
لتكوين عنصر [Range](/cells/ar/python-net/aspose.cells/range) من نطاق من الخلايا.


###  عائدات

عنصر [Range](/cells/ar/python-net/aspose.cells/range)


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_cell | str | اسم الخلية العلوي الأيسر.|
| lower_right_cell | str | أسفل اسم الخلية الأيمن.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
لتكوين عنصر [Range](/cells/ar/python-net/aspose.cells/range) من صفوف خلايا أو أعمدة خلايا.


###  عائدات

عنصر [Range](/cells/ar/python-net/aspose.cells/range).


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| first_index | int | فهرس الصف الأول أو فهرس العمود الأول ، مستند إلى الصفر.|
| number | int | إجمالي عدد الصفوف أو الأعمدة ، على أساس واحد.|
| is_vertical | bool | صواب - نطاق تم إنشاؤه من أعمدة الخلايا. خطأ - النطاق الذي تم إنشاؤه من صفوف الخلايا.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
لتكوين عنصر [Range](/cells/ar/python-net/aspose.cells/range) من نطاق من الخلايا.


###  عائدات

عنصر [Range](/cells/ar/python-net/aspose.cells/range)


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| first_row | int | الصف الأول من هذا النطاق|
| first_column | int | العمود الأول من هذا النطاق|
| total_rows | int | عدد الصفوف|
| total_columns | int | عدد الأعمدة|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)
* فئة [Range](/cells/ar/python-net/aspose.cells/range)
