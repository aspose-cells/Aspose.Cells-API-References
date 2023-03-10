---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field_name | str | اسم PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field_index | int | فهرس PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field | aspose.cells.pivot.PivotField | PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field_name | str | اسم PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field_index | int | فهرس PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر الجدول الزمني add الجديد


```python
def add(self, pivot, row, column, base_field):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني.|
| base_field | aspose.cells.pivot.PivotField | PivotField في PivotTable.BaseFields|

###  مثال

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  أنظر أيضا
* وحدة [aspose.cells.timelines](../../)
* فئة [TimelineCollection](/cells/ar/python-net/aspose.cells.timelines/timelinecollection)
