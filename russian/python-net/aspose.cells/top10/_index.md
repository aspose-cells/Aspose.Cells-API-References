---
title: Top10 класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1480
url: /ru/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 класс
 Опишите правило условного форматирования Top10.
Это правило условного форматирования выделяет ячейки,
значения попадают в верхнюю N или нижнюю N скобку, как указано.



Тип Top10 предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [Top10()](/cells/ru/python-net/aspose.cells/top10/__init__/#) |Создает новый экземпляр Top10|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_percent](/cells/ru/python-net/aspose.cells/top10/is_percent) | Получите или задайте, является ли правило "первые/нижние n" правилом "первые/нижние n процентов".<br/> Значение по умолчанию — ложь.|
| [is_bottom](/cells/ru/python-net/aspose.cells/top10/is_bottom) | Получите или задайте, является ли правило "первые/нижние n" правилом "нижних n".<br/> Значение по умолчанию — ложь.|
| [rank](/cells/ru/python-net/aspose.cells/top10/rank) | Получите или задайте значение «n» в правиле условного форматирования «верхнее/нижнее n».<br/>Если IsPercent имеет значение true, значение должно находиться в диапазоне от 0 до 100.<br/>В противном случае он должен быть между 0 и 1000.<br/> Значение по умолчанию — 10.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)
