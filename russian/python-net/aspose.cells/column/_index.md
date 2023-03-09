---
title: Column класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 260
url: /ru/python-net/aspose.cells/column/
is_root: false
---
##  Column класс
Представляет один столбец на листе.



Тип Column предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [index](/cells/ru/python-net/aspose.cells/column/index) | Получает индекс этого столбца.|
| [width](/cells/ru/python-net/aspose.cells/column/width) | Получает и задает ширину столбца в символьных единицах.|
| [group_level](/cells/ru/python-net/aspose.cells/column/group_level) |Получает уровень группы столбца.|
| [is_hidden](/cells/ru/python-net/aspose.cells/column/is_hidden) | Указывает, скрыт ли столбец.|
| [has_custom_style](/cells/ru/python-net/aspose.cells/column/has_custom_style) | Указывает, имеет ли этот столбец настраиваемые параметры стиля (отличные от стиля по умолчанию, унаследованного от рабочей книги).|
| [style](/cells/ru/python-net/aspose.cells/column/style) | Получает стиль этого столбца.|
| [is_collapsed](/cells/ru/python-net/aspose.cells/column/is_collapsed) | свернута ли колонка|


###  Методы
| Метод| Описание|
| :- | :- |
| [apply_style(style, flag)](/cells/ru/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Применяет форматы ко всему столбцу.|
| [get_style()](/cells/ru/python-net/aspose.cells/column/get_style/#) | Получает стиль этого столбца.|
| [set_style(style)](/cells/ru/python-net/aspose.cells/column/set_style/#Style) | Задает стиль этого столбца.|



###  Примеры

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

###  Смотрите также
* модуль [aspose.cells](..)
