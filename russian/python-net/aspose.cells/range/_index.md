---
title: Range класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1250
url: /ru/python-net/aspose.cells/range/
is_root: false
---
##  Range класс
Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.



Тип Range предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [current_region](/cells/ru/python-net/aspose.cells/range/current_region) |Возвращает объект Range, представляющий текущий регион.<br/> Текущая область — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов.|
| [hyperlinks](/cells/ru/python-net/aspose.cells/range/hyperlinks) | Получает все гиперссылки в диапазоне.|
| [row_count](/cells/ru/python-net/aspose.cells/range/row_count) | Получает количество строк в диапазоне.|
| [column_count](/cells/ru/python-net/aspose.cells/range/column_count) | Получает количество столбцов в диапазоне.|
| [cell_count](/cells/ru/python-net/aspose.cells/range/cell_count) | Получает количество всех ячеек в диапазоне.|
| [name](/cells/ru/python-net/aspose.cells/range/name) | Получает или задает имя диапазона.|
| [refers_to](/cells/ru/python-net/aspose.cells/range/refers_to) | Получает ссылки на диапазон.|
| [address](/cells/ru/python-net/aspose.cells/range/address) | Получает адрес диапазона.|
| [left](/cells/ru/python-net/aspose.cells/range/left) | Получает расстояние в пунктах от левого края столбца A до левого края диапазона.|
| [top](/cells/ru/python-net/aspose.cells/range/top) | Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона.|
| [width](/cells/ru/python-net/aspose.cells/range/width) | Получает ширину диапазона в пунктах.|
| [height](/cells/ru/python-net/aspose.cells/range/height) | Получает ширину диапазона в пунктах.|
| [first_row](/cells/ru/python-net/aspose.cells/range/first_row) | Получает индекс первой строки диапазона.|
| [first_column](/cells/ru/python-net/aspose.cells/range/first_column) | Получает индекс первого столбца диапазона.|
| [value](/cells/ru/python-net/aspose.cells/range/value) | Получает и задает значение диапазона.|
| [column_width](/cells/ru/python-net/aspose.cells/range/column_width) | Задает или получает ширину столбца этого диапазона|
| [row_height](/cells/ru/python-net/aspose.cells/range/row_height) | Задает или получает высоту строк в этом диапазоне|
| [entire_column](/cells/ru/python-net/aspose.cells/range/entire_column) | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон.|
| [entire_row](/cells/ru/python-net/aspose.cells/range/entire_row) | Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон.|
| [worksheet](/cells/ru/python-net/aspose.cells/range/worksheet) | Получает объект [Range.worksheet](/cells/ru/python-net/aspose.cells/range#worksheet), содержащий этот диапазон.|


###  Методы
| Метод| Описание|
| :- | :- |
| [auto_fill(target)](/cells/ru/python-net/aspose.cells/range/auto_fill/#Range) | Автоматическое заполнение целевого диапазона.|
| [auto_fill(target, auto_fill_type)](/cells/ru/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Автоматическое заполнение целевого диапазона.|
| [set_style(style, explicit_flag)](/cells/ru/python-net/aspose.cells/range/set_style/#Style-bool) | Примените стиль ячейки.|
| [set_style(style)](/cells/ru/python-net/aspose.cells/range/set_style/#Style) | Устанавливает стиль диапазона.|
| [set_outline_borders(border_style, border_color)](/cells/ru/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Устанавливает границы контура вокруг диапазона ячеек с одинаковым стилем и цветом границы.|
| [set_outline_borders(border_style, border_color)](/cells/ru/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Устанавливает границы контура вокруг диапазона ячеек с одинаковым стилем и цветом границы.|
| [set_outline_borders(border_styles, border_colors)](/cells/ru/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Устанавливает границы линии вокруг диапазона ячеек.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/ru/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Устанавливает границу контура вокруг диапазона ячеек.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/ru/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Устанавливает границу контура вокруг диапазона ячеек.|
| [copy(range, options)](/cells/ru/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Копирование диапазона со специальными параметрами вставки.|
| [copy(range)](/cells/ru/python-net/aspose.cells/range/copy/#Range) | Копирует данные (включая формулы), форматирование, объекты рисования и т. д. из исходного диапазона.|
| [get_enumerator()](/cells/ru/python-net/aspose.cells/range/get_enumerator/#) | Получает перечислитель для ячеек в этом диапазоне.|
| [is_intersect(range)](/cells/ru/python-net/aspose.cells/range/is_intersect/#Range) | Указывает, является ли диапазон пересекающимся.|
| [intersect(range)](/cells/ru/python-net/aspose.cells/range/intersect/#Range) |Возвращает объект [Range](/cells/ru/python-net/aspose.cells/range), представляющий прямоугольное пересечение двух диапазонов.|
| [union(range)](/cells/ru/python-net/aspose.cells/range/union/#Range) | Возвращает объединение двух диапазонов.|
| [merge()](/cells/ru/python-net/aspose.cells/range/merge/#) | Объединяет диапазон ячеек в одну ячейку.|
| [un_merge()](/cells/ru/python-net/aspose.cells/range/un_merge/#) | Разъединяет объединенные ячейки этого диапазона.|
| [put_value(string_value, is_converted, set_style)](/cells/ru/python-net/aspose.cells/range/put_value/#str-bool-bool) | Помещает значение в диапазон, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.|
| [apply_style(style, flag)](/cells/ru/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Применяет форматы ко всему диапазону.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/ru/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Установить внутренние границы диапазона.|
| [move_to(dest_row, dest_column)](/cells/ru/python-net/aspose.cells/range/move_to/#int-int) | Переместите текущий диапазон в диапазон назначения.|
| [copy_data(range)](/cells/ru/python-net/aspose.cells/range/copy_data/#Range) | Копирует данные ячейки (включая формулы) из исходного диапазона.|
| [copy_value(range)](/cells/ru/python-net/aspose.cells/range/copy_value/#Range) | Копирует значение ячейки из исходного диапазона.|
| [copy_style(range)](/cells/ru/python-net/aspose.cells/range/copy_style/#Range) | Копирует настройки стиля из исходного диапазона.|
| [get_cell_or_null(row_offset, column_offset)](/cells/ru/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Получает объект [Cell](/cells/ru/python-net/aspose.cells/cell) или null в этом диапазоне.|
| [get_offset(row_offset, column_offset)](/cells/ru/python-net/aspose.cells/range/get_offset/#int-int) | Получает диапазон [Range](/cells/ru/python-net/aspose.cells/range) по смещению.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
