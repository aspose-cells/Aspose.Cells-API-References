---
title: FontSetting класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 670
url: /ru/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting класс
Представляет диапазон символов в тексте ячейки.



Тип FontSetting предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/ru/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [type](/cells/ru/python-net/aspose.cells/fontsetting/type) | Получает тип текстового узла.|
| [start_index](/cells/ru/python-net/aspose.cells/fontsetting/start_index) | Получает начальный индекс символов.|
| [length](/cells/ru/python-net/aspose.cells/fontsetting/length) | Получает длину символов.|
| [font](/cells/ru/python-net/aspose.cells/fontsetting/font) | Возвращает шрифт этого объекта.|
| [text_options](/cells/ru/python-net/aspose.cells/fontsetting/text_options) |Возвращает параметры текста.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_word_art_style(style)](/cells/ru/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Задает предустановленный стиль WordArt.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)
