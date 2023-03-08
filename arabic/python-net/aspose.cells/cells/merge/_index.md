---
title: طريقة merge
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 790
url: /ar/python-net/aspose.cells/cells/merge/
is_root: false
---
##  merge(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
يدمج نطاقًا محددًا من الخلايا في خلية واحدة.



```python
def merge(self, first_row, first_column, total_rows, total_columns):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| first_row | int | الصف الأول من هذا النطاق (قائم على الصفر)|
| first_column | int | العمود الأول من هذا النطاق (على أساس الصفر)|
| total_rows | int | عدد الصفوف (واحد على أساس)|
| total_columns | int | عدد الأعمدة (واحد قائم)|
###  ملاحظات

قم بالإشارة إلى الخلية المدمجة عبر عنوان الخلية العلوية اليسرى في النطاق.

##  merge(first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}

يدمج نطاقًا محددًا من الخلايا في خلية واحدة.



```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| first_row | int | الصف الأول من هذا النطاق (قائم على الصفر)|
| first_column | int | العمود الأول من هذا النطاق (على أساس الصفر)|
| total_rows | int | عدد الصفوف (واحد على أساس)|
| total_columns | int | عدد الأعمدة (واحد قائم)|
| merge_conflict | bool | دمج النطاقات المدمجة.|
###  ملاحظات

قم بالإشارة إلى الخلية المدمجة عبر عنوان الخلية العلوية اليسرى في النطاق.
إذا كان mergeConflict صحيحًا وكان النطاق المدمج يتعارض مع الخلايا المدمجة الأخرى ،
ستتم إزالة الخلايا المدمجة الأخرى تلقائيًا.

##  merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
يدمج نطاقًا محددًا من الخلايا في خلية واحدة.



```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| first_row | int | الصف الأول من هذا النطاق (قائم على الصفر)|
| first_column | int | العمود الأول من هذا النطاق (على أساس الصفر)|
| total_rows | int | عدد الصفوف (واحد على أساس)|
| total_columns | int | عدد الأعمدة (واحد قائم)|
| check_conflict | bool | يشير إلى ما إذا كان التحقق من الخلايا المدمجة يتقاطع مع الخلايا المدمجة الأخرى|
| merge_conflict | bool | دمج النطاقات المدمجة.|
###  ملاحظات

قم بالإشارة إلى الخلية المدمجة عبر عنوان الخلية العلوية اليسرى في النطاق.
إذا كان mergeConflict صحيحًا وكان النطاق المدمج يتعارض مع الخلايا المدمجة الأخرى ،
ستتم إزالة الخلايا المدمجة الأخرى تلقائيًا.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)
