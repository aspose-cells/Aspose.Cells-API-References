---
title: FontSetting الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 670
url: /ar/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting الدرجة
يمثل مجموعة من الأحرف داخل نص الخلية.



يكشف نوع FontSetting الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/ar/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [type](/cells/ar/python-net/aspose.cells/fontsetting/type) | يحصل على نوع العقدة النصية.|
| [start_index](/cells/ar/python-net/aspose.cells/fontsetting/start_index) | يحصل على فهرس بداية الشخصيات.|
| [length](/cells/ar/python-net/aspose.cells/fontsetting/length) |يحصل على طول الأحرف.|
| [font](/cells/ar/python-net/aspose.cells/fontsetting/font) | إرجاع خط هذا الكائن.|
| [text_options](/cells/ar/python-net/aspose.cells/fontsetting/text_options) | إرجاع خيارات النص.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_word_art_style(style)](/cells/ar/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | يعيّن نمط WordArt المعين مسبقًا.|



###  أمثلة

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Visit Aspose!")
# getting charactor
charactor = cell.characters(6, 7)
# Setting the font of selected characters to bold
charactor.font.is_bold = True
# Setting the font color of selected characters to blue
charactor.font.color = Color.blue
# Saving the Excel file
workbook.save("book1.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
