---
title: PivotFormatCondition класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells.pivot/pivotformatcondition/
is_root: false
---
##  PivotFormatCondition класс
Представляет условие формата сводной таблицы в коллекции PivotFormatCondition.



Тип PivotFormatCondition предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [scope_type](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/scope_type) | Получите и задайте тип области для формата условия сводной таблицы.|
| [rule_type](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/rule_type) | Получить и установить тип правила для формата условия сводной таблицы.|
| [format_conditions](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/format_conditions) | Получите formatconditions для формата условия сводной таблицы.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_data_area_condition(field_name)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_data_area_condition/#str) | Добавляет ограничение условного формата сводной таблицы в поля данных.|
| [add_data_area_condition(data_field)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_data_area_condition/#PivotField) | Добавляет ограничение условного формата сводной таблицы в поля данных.|
| [add_row_area_condition(field_name)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_row_area_condition/#str) | Добавляет ограничение условного формата сводной таблицы в поля строки.|
| [add_row_area_condition(row_field)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_row_area_condition/#PivotField) | Добавляет ограничение условного формата сводной таблицы в поля строки.|
| [add_column_area_condition(field_name)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_column_area_condition/#str) | Добавляет ограничение условного формата сводной таблицы в полях столбца.|
| [add_column_area_condition(column_field)](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/add_column_area_condition/#PivotField) | Добавляет ограничение условного формата сводной таблицы в полях столбца.|
| [set_conditional_areas()](/cells/ru/python-net/aspose.cells.pivot/pivotformatcondition/set_conditional_areas/#) | Задает условные области объекта PivotFormatCondition.|



###  Пример

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.pivot](..)
