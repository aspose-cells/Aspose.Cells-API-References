---
title: Column الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 260
url: /ar/python-net/aspose.cells/column/
is_root: false
---
##  Column الدرجة
يمثل عمودًا واحدًا في ورقة عمل.



يكشف نوع Column الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [index](/cells/ar/python-net/aspose.cells/column/index) | يحصل على فهرس هذا العمود.|
| [width](/cells/ar/python-net/aspose.cells/column/width) | الحصول على عرض العمود وتعيينه بوحدة من الأحرف.|
| [group_level](/cells/ar/python-net/aspose.cells/column/group_level) |يحصل على مستوى المجموعة للعمود.|
| [is_hidden](/cells/ar/python-net/aspose.cells/column/is_hidden) | يشير إلى ما إذا كان العمود مخفيًا.|
| [has_custom_style](/cells/ar/python-net/aspose.cells/column/has_custom_style) | يشير إلى ما إذا كان هذا العمود يحتوي على إعدادات نمط مخصصة (تختلف عن الإعداد الافتراضي الموروث من المصنف).|
| [style](/cells/ar/python-net/aspose.cells/column/style) | يحصل على نمط هذا العمود.|
| [is_collapsed](/cells/ar/python-net/aspose.cells/column/is_collapsed) | ما إذا كان العمود مطويًا أم لا|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [apply_style(style, flag)](/cells/ar/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | يطبق تنسيقات لعمود كامل.|
| [get_style()](/cells/ar/python-net/aspose.cells/column/get_style/#) | يحصل على نمط هذا العمود.|
| [set_style(style)](/cells/ar/python-net/aspose.cells/column/set_style/#Style) | يحدد نمط هذا العمود.|



###  مثال

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
