---
title: طريقة import_custom_objects
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 640
url: /ar/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
يستورد كائنات مخصصة.


###  عائدات

إجمالي عدد الصفوف التي تم استيرادها.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| list | list | الكائن المخصص|
| first_row | int | رقم صف الخلية الأولى المطلوب الاستيراد فيها.|
| first_column | int | رقم العمود الخاص بالخلية الأولى التي سيتم الاستيراد فيها.|
| options | [ImportTableOptions](/cells/ar/python-net/aspose.cells/importtableoptions) | خيارات الاستيراد.|
###  ملاحظات

يجب أن تكون الكائنات المخصصة من نفس النوع.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

يستورد كائنات مخصصة.


###  عائدات

إجمالي عدد الصفوف التي تم استيرادها.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| list | list | الكائن المخصص|
| property_names | list | أسماء الخصائص ، إذا كانت خالية ، فسنقوم باستيراد جميع خصائص الكائن.|
| is_property_name_shown | bool | يشير إلى ما إذا كان سيتم استيراد اسم الخاصية إلى الصف الأول.|
| first_row | int | رقم صف الخلية الأولى المطلوب الاستيراد فيها.|
| first_column | int | رقم العمود الخاص بالخلية الأولى التي سيتم الاستيراد فيها.|
| row_number | int | عدد الصفوف المراد استيرادها.|
| insert_rows | bool | يشير إلى ما إذا كانت الصفوف الإضافية ستتم إضافتها لملاءمة البيانات.|
| date_format_string | str | سلسلة تنسيق التاريخ للخلايا.|
| convert_string_to_number | bool | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل سلسلة إلى رقم.|
###  ملاحظات

يجب أن تكون الكائنات المخصصة من نفس النوع.


###  أنظر أيضا

* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)
