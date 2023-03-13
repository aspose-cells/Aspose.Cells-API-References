---
title: AbstractCalculationMonitor класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor класс
Монитор для пользователя, чтобы отслеживать ход расчета формулы.



Тип AbstractCalculationMonitor предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [original_value](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Получает старое значение вычисляемой ячейки.<br/> Следует использовать только в [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) и [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Было ли изменено значение ячейки после вычисления.<br/> Следует использовать только в [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Получает новое вычисленное значение ячейки.<br/> Следует использовать только в [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  Методы
| Метод| Описание|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Реализуйте этот метод для ведения бизнеса перед расчетом одной ячейки.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Реализуйте этот метод для ведения бизнеса после того, как будет рассчитана одна ячейка.|
| [on_circular(circular_cells_data)](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Реализуйте этот метод для ведения бизнеса при расчете формул с циклическими ссылками.|



###  Смотрите также
* модуль [aspose.cells](..)
