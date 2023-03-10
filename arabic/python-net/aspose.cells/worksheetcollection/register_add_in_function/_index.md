---
title: طريقة register_add_in_function
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 170
url: /ar/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
يضيف وظيفة الوظيفة الإضافية في المصنف


###  عائدات

عنوان URL لملف الوظيفة الإضافية الذي يحتوي على وظائف الوظيفة الإضافية


```python
def register_add_in_function(self, id, function_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| id | int | معرف البيانات التي تحتوي على وظائف إضافية ،<br/> يمكن الحصول عليها من خلال المكالمة الأولى من [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/ar/python-net/aspose.cells/worksheetcollection/register_add_in_function) لنفس ملف الوظيفة الإضافية.|
| function_name | str | اسم وظيفة الوظيفة الإضافية|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
يضيف وظيفة الوظيفة الإضافية في المصنف


###  عائدات

معرف البيانات التي تحتوي على وظيفة إضافية معينة


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| add_in_file | str | يحتوي الملف على وظائف الوظيفة الإضافية|
| function_name | str | اسم وظيفة الوظيفة الإضافية|
| lib | bool | ما إذا كان الملف الإضافي المحدد موجودًا في الدليل أو الدليل الفرعي لمكتبة Workbook Add-In.<br/>تسري هذه العلامة وتحدث فرقًا عندما يكون ملف addIn المعطى ذا مسار نسبي:<br/> تشير القيمة true إلى أن المسار متعلق بمكتبة الوظائف الإضافية بينما تشير القيمة false إلى أن المسار مرتبط بهذا المصنف.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [WorksheetCollection](/cells/ar/python-net/aspose.cells/worksheetcollection)
