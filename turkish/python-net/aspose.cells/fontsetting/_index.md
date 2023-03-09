---
title: FontSetting sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 670
url: /tr/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting sınıfı
Hücre metni içindeki bir karakter aralığını temsil eder.



FontSetting türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/tr/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [type](/cells/tr/python-net/aspose.cells/fontsetting/type) | Metin düğümü türünü alır.|
| [start_index](/cells/tr/python-net/aspose.cells/fontsetting/start_index) | Karakterlerin başlangıç dizinini alır.|
| [length](/cells/tr/python-net/aspose.cells/fontsetting/length) |Karakterlerin uzunluklarını alır.|
| [font](/cells/tr/python-net/aspose.cells/fontsetting/font) | Bu nesnenin yazı tipini döndürür.|
| [text_options](/cells/tr/python-net/aspose.cells/fontsetting/text_options) | Metin seçeneklerini döndürür.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_word_art_style(style)](/cells/tr/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Önceden ayarlanmış WordArt stilini ayarlar.|



###  örnekler

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

###  Ayrıca bakınız
* modül [aspose.cells](..)
