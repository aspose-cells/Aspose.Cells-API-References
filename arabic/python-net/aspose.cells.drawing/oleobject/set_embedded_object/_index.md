---
title: طريقة set_embedded_object
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 170
url: /ar/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
يضبط بيانات الكائن المضمنة.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| link_to_file | bool | يشير إلى ما إذا كان الكائن مرتبطًا بالملف. إذا كان هذا صحيحًا ، فسيتم تجاهل المعلمة objectData.|
| object_data | bytes | بيانات الكائن المضمنة.|
| source_file_name | str | اسم الملف.|
| display_as_icon | bool | يشير إلى ما إذا كان كائن دبلجة كرمز.<br/> إذا كان هذا صحيحًا ، فستتم تغطية بيانات الصورة الأصلية بالرمز.|
| label | str | تسمية الرمز. يعمل فقط عندما تكون قيمة displayAsIcon صحيحة.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
يضبط بيانات الكائن المضمنة.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| link_to_file | bool | يشير إلى ما إذا كان الكائن مرتبطًا بالملف. إذا كان هذا صحيحًا ، فسيتم تجاهل المعلمة objectData.|
| object_data | bytes | بيانات الكائن المضمنة.|
| source_file_name | str | اسم الملف.|
| display_as_icon | bool | يشير إلى ما إذا كان كائن دبلجة كرمز.<br/> إذا كان هذا صحيحًا ، فستتم تغطية بيانات الصورة الأصلية بالرمز.|
| label | str | تسمية الرمز. يعمل فقط عندما تكون قيمة displayAsIcon صحيحة.|
| update_icon | bool | يشير إلى ما إذا كان يتم تحديث الرمز تلقائيًا.|
###  ملاحظات

نظرًا لأن Aspose يمكنه تحديث تضمين كافة أيقونات الملفات ، فمن الأفضل إضافة رمز صحيح مع وجود `update_icon` على أنه خطأ.


###  أنظر أيضا

* وحدة [aspose.cells.drawing](../../)
* فئة [OleObject](/cells/ar/python-net/aspose.cells.drawing/oleobject)
