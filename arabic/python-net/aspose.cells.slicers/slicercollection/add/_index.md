---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض.|
| base_field_name | str | اسم PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض.|
| base_field_index | int | فهرس PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| dest_cell_name | str | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض.|
| base_field | aspose.cells.pivot.PivotField | PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
أضف أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, table, index, dest_cell_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | كائن ListObject|
| index | int | فهرس ListColumn في ListObject.ListColumns|
| dest_cell_name | str | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض.|

###  أمثلة

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
أضف أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | كائن ListObject|
| list_column | aspose.cells.tables.ListColumn | يعد ListColumn في ListObject.ListColumns|
| dest_cell_name | str | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض.|

###  أمثلة

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة.|
| base_field_name | str | اسم PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة.|
| base_field_index | int | فهرس PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
إضافة Slicer جديد باستخدام PivotTable كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, pivot, row, column, base_field):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |كائن PivotTable|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة.|
| base_field | aspose.cells.pivot.PivotField | PivotField في PivotTable.BaseFields|

###  أمثلة

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
أضف أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات


###  عائدات

مؤشر تقطيع add الجديد


```python
def add(self, table, list_column, row, column):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | كائن ListObject|
| list_column | aspose.cells.tables.ListColumn | يعد ListColumn في ListObject.ListColumns|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح.|
| column | int | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة.|

###  أمثلة

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



###  أنظر أيضا
* وحدة [aspose.cells.slicers](../../)
* فئة [SlicerCollection](/cells/ar/python-net/aspose.cells.slicers/slicercollection)
