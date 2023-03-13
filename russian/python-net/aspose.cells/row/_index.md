---
title: Row класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1300
url: /ru/python-net/aspose.cells/row/
is_root: false
---
##  Row класс
Представляет одну строку на листе.



Тип Row предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_blank](/cells/ru/python-net/aspose.cells/row/is_blank) | Указывает, содержит ли строка какие-либо данные|
| [is_collapsed](/cells/ru/python-net/aspose.cells/row/is_collapsed) | свернута ли строка|
| [height](/cells/ru/python-net/aspose.cells/row/height) | Получает и задает высоту строки в пунктах.|
| [is_hidden](/cells/ru/python-net/aspose.cells/row/is_hidden) | Указывает, скрыта ли строка.|
| [index](/cells/ru/python-net/aspose.cells/row/index) | Получает индекс этой строки.|
| [group_level](/cells/ru/python-net/aspose.cells/row/group_level) | Получает уровень группы строки.|
| [is_height_matched](/cells/ru/python-net/aspose.cells/row/is_height_matched) |Указывает, что высота строки и высота шрифта по умолчанию совпадают.|
| [style](/cells/ru/python-net/aspose.cells/row/style) | Представляет стиль этой строки.|
| [has_custom_style](/cells/ru/python-net/aspose.cells/row/has_custom_style) | Указывает, есть ли в этой строке пользовательские настройки стиля (отличные от настроек по умолчанию, унаследованных от книги).|
| [first_cell](/cells/ru/python-net/aspose.cells/row/first_cell) | Получает первый объект ячейки в строке.|
| [first_data_cell](/cells/ru/python-net/aspose.cells/row/first_data_cell) | Получает первую непустую ячейку в строке.|
| [last_cell](/cells/ru/python-net/aspose.cells/row/last_cell) | Получает последний объект ячейки в строке.|
| [last_data_cell](/cells/ru/python-net/aspose.cells/row/last_data_cell) | Получает последнюю непустую ячейку в строке.|



Получает ячейку.
###  Индексатор
| Имя| Описание|
| :- | :- |
| [index] | Индекс столбца|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_cell_by_index(index)](/cells/ru/python-net/aspose.cells/row/get_cell_by_index/#int) | Получить ячейку по определенному индексу в списке.|
| [get_cell_or_null(column)](/cells/ru/python-net/aspose.cells/row/get_cell_or_null/#int) | Получает ячейку или null в указанном индексе.|
| [get_style()](/cells/ru/python-net/aspose.cells/row/get_style/#) | Получает стиль этой строки.|
| [set_style(style)](/cells/ru/python-net/aspose.cells/row/set_style/#Style) | Устанавливает стиль этой строки.|
| [copy_settings(source, check_style)](/cells/ru/python-net/aspose.cells/row/copy_settings/#Row-bool) | Скопируйте настройки строки, такие как стиль, высота, видимость и т. д.|
| [apply_style(style, flag)](/cells/ru/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Применяет форматы ко всей строке.|
| [equals(row)](/cells/ru/python-net/aspose.cells/row/equals/#Row) | Проверяет, ссылается ли этот объект на ту же строку с другим объектом строки.|



###  Пример

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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
