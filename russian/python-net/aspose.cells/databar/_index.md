---
title: DataBar класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 400
url: /ru/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar класс
 Опишите правило условного форматирования DataBar.
Это правило условного форматирования отображает градуированный
панель данных в диапазоне ячеек.



Тип DataBar предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [axis_color](/cells/ru/python-net/aspose.cells/databar/axis_color) | Получает цвет оси для ячеек с условным форматированием в виде гистограмм.|
| [axis_position](/cells/ru/python-net/aspose.cells/databar/axis_position) | Получает или задает положение оси гистограмм, заданное правилом условного форматирования.|
| [bar_fill_type](/cells/ru/python-net/aspose.cells/databar/bar_fill_type) | Получает или задает способ заполнения панели данных цветом.|
| [direction](/cells/ru/python-net/aspose.cells/databar/direction) |Получает или задает направление отображения панели данных.|
| [bar_border](/cells/ru/python-net/aspose.cells/databar/bar_border) | Получает объект, указывающий границу гистограммы.|
| [negative_bar_format](/cells/ru/python-net/aspose.cells/databar/negative_bar_format) | Получает объект NegativeBarFormat, связанный с правилом условного форматирования гистограммы.|
| [min_cfvo](/cells/ru/python-net/aspose.cells/databar/min_cfvo) | Получите или установите объект минимального значения этого DataBar.<br/> Невозможно установить значение null или CFValueObject с типом FormatConditionValueType.Max.|
| [max_cfvo](/cells/ru/python-net/aspose.cells/databar/max_cfvo) | Получите или установите объект максимального значения этого DataBar.<br/> Невозможно установить значение null или CFValueObject с типом FormatConditionValueType.Min.|
| [color](/cells/ru/python-net/aspose.cells/databar/color) | Получить или установить цвет этого DataBar.|
| [min_length](/cells/ru/python-net/aspose.cells/databar/min_length) | Представляет минимальную длину строки данных.|
| [max_length](/cells/ru/python-net/aspose.cells/databar/max_length) | Представляет максимальную длину строки данных.|
| [show_value](/cells/ru/python-net/aspose.cells/databar/show_value) | Получите или установите флаг, указывающий, следует ли отображать значения ячеек, к которым применяется эта панель данных.<br/> Значение по умолчанию — истина.|


###  Методы
| Метод| Описание|
| :- | :- |
| [to_image(cell, img_opts)](/cells/ru/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Отобразите панель данных в ячейке в массив байтов изображения.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)
