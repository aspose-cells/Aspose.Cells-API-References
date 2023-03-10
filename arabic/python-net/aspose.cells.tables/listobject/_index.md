---
title: ListObject الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject الدرجة
يمثل كائن قائمة في ورقة عمل.
 الكائن ListObject هو عضو في مجموعة ListObjects.
تحتوي مجموعة ListObjects على كافة كائنات القائمة في ورقة العمل.



يكشف نوع ListObject الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [start_row](/cells/ar/python-net/aspose.cells.tables/listobject/start_row) | يحصل على صف البداية للنطاق.|
| [start_column](/cells/ar/python-net/aspose.cells.tables/listobject/start_column) | يحصل على عمود البداية للنطاق.|
| [end_row](/cells/ar/python-net/aspose.cells.tables/listobject/end_row) | يحصل على صف نهاية النطاق.|
| [end_column](/cells/ar/python-net/aspose.cells.tables/listobject/end_column) |يحصل على عمود نهاية النطاق.|
| [list_columns](/cells/ar/python-net/aspose.cells.tables/listobject/list_columns) | يحصل على ListColumns من ListObject.|
| [show_header_row](/cells/ar/python-net/aspose.cells.tables/listobject/show_header_row) | الحصول على وتحديد ما إذا كان ListObject هذا يعرض صف الرأس أم لا.|
| [show_totals](/cells/ar/python-net/aspose.cells.tables/listobject/show_totals) | الحصول على وتحديد ما إذا كان ListObject هذا يعرض صف الإجمالي أم لا.|
| [data_range](/cells/ar/python-net/aspose.cells.tables/listobject/data_range) | يحصل على نطاق بيانات ListObject.|
| [query_table](/cells/ar/python-net/aspose.cells.tables/listobject/query_table) | يحصل على QueryTable المرتبط.|
| [data_source_type](/cells/ar/python-net/aspose.cells.tables/listobject/data_source_type) | يحصل على نوع مصدر البيانات الخاص بالجدول.|
| [auto_filter](/cells/ar/python-net/aspose.cells.tables/listobject/auto_filter) | يحصل على مرشح تلقائي.|
| [display_name](/cells/ar/python-net/aspose.cells.tables/listobject/display_name) | الحصول على اسم العرض وتعيينه.|
| [comment](/cells/ar/python-net/aspose.cells.tables/listobject/comment) | يحصل ويضع تعليق الجدول.|
| [show_table_style_first_column](/cells/ar/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | يشير إلى ما إذا كان يجب تطبيق النمط على العمود الأول في الجدول.|
| [show_table_style_last_column](/cells/ar/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | يشير إلى ما إذا كان يجب تطبيق النمط على العمود الأخير في الجدول.|
| [show_table_style_row_stripes](/cells/ar/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | الإشارة إلى ما إذا كان تنسيق شريط الصفوف مطبقًا أم لا.|
| [show_table_style_column_stripes](/cells/ar/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا أم لا.|
| [table_style_type](/cells/ar/python-net/aspose.cells.tables/listobject/table_style_type) | يحصل وأسلوب الجدول المدمج.|
| [table_style_name](/cells/ar/python-net/aspose.cells.tables/listobject/table_style_name) | الحصول على اسم نمط الجدول وتعيينه.|
| [xml_map](/cells/ar/python-net/aspose.cells.tables/listobject/xml_map) | الحصول على [ListObject.xml_map](/cells/ar/python-net/aspose.cells.tables/listobject#xml_map) المستخدم لهذه القائمة.|
| [alternative_text](/cells/ar/python-net/aspose.cells.tables/listobject/alternative_text) | يحصل على النص البديل ويضعه.|
| [alternative_description](/cells/ar/python-net/aspose.cells.tables/listobject/alternative_description) | يحصل ويضع الوصف البديل.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [convert_to_range()](/cells/ar/python-net/aspose.cells.tables/listobject/convert_to_range/#) | تحويل الجدول إلى نطاق.|
| [convert_to_range(options)](/cells/ar/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | تحويل الجدول إلى نطاق.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/ar/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | تغيير حجم نطاق كائن القائمة.|
| [put_cell_value(row_offset, column_offset, value)](/cells/ar/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | ضع القيمة على الخلية.|
| [update_column_name()](/cells/ar/python-net/aspose.cells.tables/listobject/update_column_name/#) |يحدّث جميع أسماء أعمدة القائمة من ورقة العمل.|
| [filter()](/cells/ar/python-net/aspose.cells.tables/listobject/filter/#) | تصفية الجدول.|
| [apply_style_to_range()](/cells/ar/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | قم بتطبيق نمط الجدول على النطاق.|



###  مثال

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.tables](..)
