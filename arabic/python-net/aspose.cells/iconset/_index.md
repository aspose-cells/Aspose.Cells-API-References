---
title: IconSet الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 900
url: /ar/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet الدرجة
 صِف قاعدة التنسيق الشرطي IconSet.
تطبق قاعدة التنسيق الشرطي هذه الرموز على الخلايا
وفقًا لقيمهم.



يكشف نوع IconSet الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [cf_icons](/cells/ar/python-net/aspose.cells/iconset/cf_icons) | احصل على[ConditionalFormattingIcon](/cells/ar/python-net/aspose.cells/conditionalformattingicon) من المجموعة|
| [cfvos](/cells/ar/python-net/aspose.cells/iconset/cfvos) | احصل على مثيل CFValueObjects.|
| [type](/cells/ar/python-net/aspose.cells/iconset/type) | احصل على نوع مجموعة الرموز المراد عرضها أو اضبطها.<br/>سيؤدي تعيين النوع إلى التحقق تلقائيًا مما إذا كان عدد Cfvos الحالي هو<br/> تتفق مع النوع الجديد. إذا لم يتم التوافق ، فسيتم تنظيف Cfvos القديم و<br/> ستتم إضافة Cfvos الافتراضية.|
| [is_custom](/cells/ar/python-net/aspose.cells/iconset/is_custom) | يشير إلى ما إذا كانت مجموعة الرموز مخصصة.<br/> القيمة الافتراضية هي كاذبة.|
| [show_value](/cells/ar/python-net/aspose.cells/iconset/show_value) | احصل على أو عيّن العلامة التي تشير إلى ما إذا كنت تريد إظهار قيم الخلايا التي يتم تطبيق مجموعة الأيقونات عليها.<br/> القيمة الافتراضية صحيحة.|
| [reverse](/cells/ar/python-net/aspose.cells/iconset/reverse) | احصل على أو اضبط العلم الذي يشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للرموز في مجموعة الرموز هذه.<br/> القيمة الافتراضية هي كاذبة.|



###  مثال

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

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
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
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
* فئة [ConditionalFormattingIcon](/cells/ar/python-net/aspose.cells/conditionalformattingicon)
