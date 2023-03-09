---
title: WorkbookDesigner الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1600
url: /ar/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner الدرجة
لتغليف الكائن الذي يمثل جدول بيانات المصمم.



يكشف نوع WorkbookDesigner الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [WorkbookDesigner()](/cells/ar/python-net/aspose.cells/workbookdesigner/__init__/#) | يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](/cells/ar/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/ar/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](/cells/ar/python-net/aspose.cells/workbookdesigner).|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [workbook](/cells/ar/python-net/aspose.cells/workbookdesigner/workbook) |الحصول على العنصر [WorkbookDesigner.workbook](/cells/ar/python-net/aspose.cells/workbookdesigner#workbook) وتعيينه.|
| [repeat_formulas_with_subtotal](/cells/ar/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | يشير إلى ما إذا كان يتم تكرار الصيغ مع صفوف الإجمالي الفرعي.|
| [update_empty_string_as_null](/cells/ar/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | إذا كانت القيمة TRUE ، فسيتم إدراج Null إذا كانت القيمة "" ؛|
| [update_reference](/cells/ar/python-net/aspose.cells/workbookdesigner/update_reference) |يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى.|
| [calculate_formula](/cells/ar/python-net/aspose.cells/workbookdesigner/calculate_formula) | يشير إلى ما إذا كان يجب حساب الصيغ.|
| [call_back](/cells/ar/python-net/aspose.cells/workbookdesigner/call_back) | يحصل ويعين واجهة رد معالجة سمارت ماركر.|
| [line_by_line](/cells/ar/python-net/aspose.cells/workbookdesigner/line_by_line) | يشير إلى ما إذا كانت معالجة العلامة الذكية سطرًا بسطر.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/ar/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | يحدد مصدر البيانات لكائن [ICellsDataTable](/cells/ar/python-net/aspose.cells/icellsdatatable).|
| [set_data_source(variable, data)](/cells/ar/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | يضبط ربط البيانات بمتغير.|
| [process()](/cells/ar/python-net/aspose.cells/workbookdesigner/process/#) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات.|
| [process(is_preserved)](/cells/ar/python-net/aspose.cells/workbookdesigner/process/#bool) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات.|
| [process(sheet_index, is_preserved)](/cells/ar/python-net/aspose.cells/workbookdesigner/process/#int-bool) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات.|
| [clear_data_source()](/cells/ar/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | يمسح كل مصادر البيانات.|
| [get_smart_markers()](/cells/ar/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | إرجاع مجموعة من العلامات الذكية في جدول بيانات.|



###  أمثلة

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [ICellsDataTable](/cells/ar/python-net/aspose.cells/icellsdatatable)
* فئة [WorkbookDesigner](/cells/ar/python-net/aspose.cells/workbookdesigner)
