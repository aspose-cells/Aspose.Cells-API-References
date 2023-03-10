---
title: IconSet класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 900
url: /ru/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet класс
 Опишите правило условного форматирования IconSet.
Это правило условного форматирования применяет значки к ячейкам.
в соответствии с их значениями.



Тип IconSet предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [cf_icons](/cells/ru/python-net/aspose.cells/iconset/cf_icons) | Получите [ConditionalFormattingIcon](/cells/ru/python-net/aspose.cells/conditionalformattingicon) из коллекции|
| [cfvos](/cells/ru/python-net/aspose.cells/iconset/cfvos) | Получите экземпляр CFValueObjects.|
| [type](/cells/ru/python-net/aspose.cells/iconset/type) | Получить или установить тип набора значков для отображения.<br/>Установка типа автоматически проверит, соответствует ли текущий счетчик Cfvos.<br/> соответствии с новым типом. В противном случае старые Cfvos будут очищены и<br/> будут добавлены Cfvo по умолчанию.|
| [is_custom](/cells/ru/python-net/aspose.cells/iconset/is_custom) | Указывает, является ли набор значков пользовательским.<br/> Значение по умолчанию — ложь.|
| [show_value](/cells/ru/python-net/aspose.cells/iconset/show_value) | Получите или установите флаг, указывающий, следует ли отображать значения ячеек, к которым применяется этот набор значков.<br/> Значение по умолчанию — истина.|
| [reverse](/cells/ru/python-net/aspose.cells/iconset/reverse) | Получите или установите флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков.<br/> Значение по умолчанию — ложь.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)
* класс [ConditionalFormattingIcon](/cells/ru/python-net/aspose.cells/conditionalformattingicon)
