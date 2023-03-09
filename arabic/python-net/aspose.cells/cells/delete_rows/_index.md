---
title: طريقة delete_rows
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 260
url: /ar/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
يحذف عدة صفوف.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| row_index | int |سيتم حذف فهرس الصف الأول.|
| total_rows | int | عدد الصفوف المراد حذفها.|
###  ملاحظات

إذا كان النطاق المحذوف يحتوي على الجزء العلوي (ليس بالكامل) من الجدول (ListObject) ،
النطاق لا يمكن حذفه ولن يتم عمل شيء. يعمل مثل MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
يحذف عدة صفوف من ورقة العمل.


###  عائدات




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| row_index | int | فهرس الصف.|
| total_rows | int | عدد الصفوف المراد حذفها.|
| update_reference | bool | يشير إلى ما إذا كان يتم تحديث المراجع في أوراق العمل الأخرى.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)
