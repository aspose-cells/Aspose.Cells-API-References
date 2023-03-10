---
title: FormatConditionCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 700
url: /ar/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
##  FormatConditionCollection الدرجة
يمثل التنسيق الشرطي.
يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية.



يكشف نوع FormatConditionCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [count](/cells/ar/python-net/aspose.cells/formatconditioncollection/count) | يحصل على حساب الشروط.|
| [range_count](/cells/ar/python-net/aspose.cells/formatconditioncollection/range_count) | الحصول على عدد النطاقات المنسقة شرطيًا.|



يحصل على شرط التنسيق بالفهرس.
###  مفهرس
| اسم| وصف|
| :- | :- |
| [index] | فهرس شرط التنسيق للرجوع.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/ar/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | يضيف شرط تنسيق.|
| [add_condition(type)](/cells/ar/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) |أضف شرط تنسيق.|
| [remove_area(index)](/cells/ar/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | يزيل نطاق الخلايا المنسق الشرطي بالفهرس.|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/ar/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | قم بإزالة التنسيق الشرطي في النطاق.|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/ar/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | يضيف شرط تنسيق ونطاق خلية مؤثر إلى FormatConditions<br/>يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية.<br/> غير مسموح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي.|
| [add_area(cell_area)](/cells/ar/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | يضيف نطاق خلايا منسق شرطيًا.|
| [get_cell_area(index)](/cells/ar/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | الحصول على نطاق الخلايا المنسق الشرطي حسب الفهرس.|
| [remove_condition(index)](/cells/ar/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | يزيل شرط التنسيق بالفهرس.|



###  مثال

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
