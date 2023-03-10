---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.


###  عائدات

تم إضافة فهرس ذاكرة التخزين المؤقت الجديد.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | str | بيانات ذاكرة التخزين المؤقت الجديدة لـ PivotTable.|
| dest_cell_name | str |الخلية الموجودة في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
إضافة كائن PivotTable جديد إلى المجموعة من PivotTable آخر.


###  عائدات

تمت إضافة فهرس PivotTable الجديد.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/ar/python-net/aspose.cells.pivot/pivottable) | المصدر pivotTable.|
| dest_cell_name | str |الخلية الموجودة في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.


###  عائدات

تم إضافة فهرس ذاكرة التخزين المؤقت الجديد.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | str | بيانات ذاكرة التخزين المؤقت الجديدة لـ PivotTable.|
| dest_cell_name | str |الخلية الموجودة في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|
| use_same_source | bool | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عند استخدام جدول محوري آخر لمصدر البيانات هذا.<br/> إذا كانت الخاصية صحيحة ، فسيتم حفظ الذاكرة.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.


###  عائدات

تم إضافة فهرس ذاكرة التخزين المؤقت الجديد.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | str | نطاق خلايا البيانات لجدول PivotTable الجديد. مثال: الورقة 1! A1: C8|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| column | int | فهرس عمود الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
إضافة كائن PivotTable جديد إلى المجموعة من PivotTable آخر.


###  عائدات

تمت إضافة فهرس PivotTable الجديد.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/ar/python-net/aspose.cells.pivot/pivottable) | المصدر pivotTable.|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| column | int | فهرس عمود الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.


###  عائدات

تم إضافة فهرس ذاكرة التخزين المؤقت الجديد.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | str | نطاق خلايا البيانات لجدول PivotTable الجديد. مثال: الورقة 1! A1: C8|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| column | int | فهرس عمود الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|
| use_same_source | bool | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عند استخدام جدول محوري آخر لمصدر البيانات هذا.<br/> إذا كانت الخاصية صحيحة ، فسيتم حفظ الذاكرة.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
يضيف كائن PivotTable جديدًا إلى المجموعة ذات نطاقات الدمج المتعددة كمصدر بيانات.


###  عائدات

تمت إضافة فهرس PivotTable الجديد.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | list | نطاقات الدمج المتعددة ، مثل {"Sheet1! A1: C8"، "Sheet2! A1: B8"} |
| is_auto_page | bool | ما إذا كان سيتم إنشاء حقل صفحة واحد تلقائيًا.<br/>إذا كان هذا صحيحًا ، فسيتم تجاهل معلمة pageFields التالية.|
| page_fields | [PivotPageFields](/cells/ar/python-net/aspose.cells.pivot/pivotpagefields) | عناصر حقل الصفحة المحورية.|
| dest_cell_name | str | destCellName اسم تقرير PivotTable الجديد.|
| table_name | str | اسم تقرير PivotTable الجديد.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
يضيف كائن PivotTable جديدًا إلى المجموعة ذات نطاقات الدمج المتعددة كمصدر بيانات.


###  عائدات

تمت إضافة فهرس PivotTable الجديد.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| source_data | list | نطاقات الدمج المتعددة ، مثل {"Sheet1! A1: C8"، "Sheet2! A1: B8"} |
| is_auto_page | bool | ما إذا كان سيتم إنشاء حقل صفحة واحد تلقائيًا.<br/> إذا كان هذا صحيحًا ، فسيتم تجاهل معلمة pageFields التالية|
| page_fields | [PivotPageFields](/cells/ar/python-net/aspose.cells.pivot/pivotpagefields) | عناصر حقل الصفحة المحورية.|
| row | int | فهرس صف الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| column | int | فهرس عمود الخلية في الزاوية العلوية اليسرى من النطاق الوجهة لتقرير PivotTable.|
| table_name | str | اسم تقرير PivotTable الجديد.|



###  أنظر أيضا
* وحدة [aspose.cells.pivot](../../)
* فئة [PivotTableCollection](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection)
