---
title: DataBar الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 400
url: /ar/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar الدرجة
 صِف قاعدة التنسيق الشرطي DataBar.
تعرض قاعدة التنسيق الشرطي هذه قيمة
شريط البيانات في نطاق الخلايا.



يكشف نوع DataBar الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [axis_color](/cells/ar/python-net/aspose.cells/databar/axis_color) | الحصول على لون المحور للخلايا ذات التنسيق الشرطي كأشرطة بيانات.|
| [axis_position](/cells/ar/python-net/aspose.cells/databar/axis_position) | الحصول على أو تعيين موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي.|
| [bar_fill_type](/cells/ar/python-net/aspose.cells/databar/bar_fill_type) | الحصول على أو تعيين كيفية تعبئة شريط البيانات باللون.|
| [direction](/cells/ar/python-net/aspose.cells/databar/direction) |الحصول على أو تحديد اتجاه عرض قاعدة البيانات.|
| [bar_border](/cells/ar/python-net/aspose.cells/databar/bar_border) | يحصل على كائن يحدد حدود شريط البيانات.|
| [negative_bar_format](/cells/ar/python-net/aspose.cells/databar/negative_bar_format) | الحصول على كائن NegativeBarFormat المقترن بقاعدة التنسيق الشرطي لشريط البيانات.|
| [min_cfvo](/cells/ar/python-net/aspose.cells/databar/min_cfvo) | الحصول على كائن القيمة الدنيا الخاص بـ DataBar أو تعيينه.<br/> لا يمكن تعيين القيمة null أو CFValueObject بالنوع FormatConditionValueType.Max.|
| [max_cfvo](/cells/ar/python-net/aspose.cells/databar/max_cfvo) | الحصول على كائن القيمة القصوى لـ DataBar هذا أو تعيينه.<br/> لا يمكن تعيين القيمة الخالية أو CFValueObject بالنوع FormatConditionValueType.Min إليها.|
| [color](/cells/ar/python-net/aspose.cells/databar/color) | الحصول على أو تعيين لون شريط البيانات هذا.|
| [min_length](/cells/ar/python-net/aspose.cells/databar/min_length) | يمثل الحد الأدنى لطول شريط البيانات.|
| [max_length](/cells/ar/python-net/aspose.cells/databar/max_length) | يمثل الحد الأقصى لطول شريط البيانات.|
| [show_value](/cells/ar/python-net/aspose.cells/databar/show_value) | احصل على أو عيّن العلامة التي تشير إلى ما إذا كنت تريد إظهار قيم الخلايا التي يتم تطبيق شريط البيانات عليها.<br/> القيمة الافتراضية صحيحة.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [to_image(cell, img_opts)](/cells/ar/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | تقديم شريط البيانات في الخلية إلى مصفوفة بايت الصورة.|



###  أمثلة

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
