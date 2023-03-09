---
title: Top10 الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1480
url: /ar/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 الدرجة
 صِف قاعدة التنسيق الشرطي Top10.
تسلط قاعدة التنسيق الشرطي هذه الضوء على الخلايا التي تحتوي على
تقع القيم في أعلى قوس N أو أسفل N ، كما هو محدد.



يكشف نوع Top10 الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [Top10()](/cells/ar/python-net/aspose.cells/top10/__init__/#) |يقوم بإنشاء مثيل جديد لـ Top10|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_percent](/cells/ar/python-net/aspose.cells/top10/is_percent) | الحصول على أو تحديد ما إذا كانت قاعدة "أعلى / أسفل" قاعدة "أعلى / أسفل ن" قاعدة.<br/> القيمة الافتراضية هي كاذبة.|
| [is_bottom](/cells/ar/python-net/aspose.cells/top10/is_bottom) | احصل على أو عيّن ما إذا كانت قاعدة "أعلى / أسفل" قاعدة "سفلية".<br/> القيمة الافتراضية هي كاذبة.|
| [rank](/cells/ar/python-net/aspose.cells/top10/rank) | الحصول على قيمة "n" أو تعيينها في قاعدة التنسيق الشرطي "top / bottom n".<br/>إذا كانت IsPercent صحيحة ، فيجب أن تكون القيمة بين 0 و 100.<br/>وإلا يجب أن يكون بين 0 و 1000.<br/> القيمة الافتراضية هي 10.|



###  أمثلة

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
