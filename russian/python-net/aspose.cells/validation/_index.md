---
title: Validation класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1540
url: /ru/python-net/aspose.cells/validation/
is_root: false
---
##  Validation класс
Представляет данные validation.settings.



Тип Validation предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [operator](/cells/ru/python-net/aspose.cells/validation/operator) | Представляет оператор для проверки данных.|
| [alert_style](/cells/ru/python-net/aspose.cells/validation/alert_style) | Представляет стиль оповещения о проверке.|
| [type](/cells/ru/python-net/aspose.cells/validation/type) | Представляет тип проверки данных.|
| [input_message](/cells/ru/python-net/aspose.cells/validation/input_message) | Представляет входное сообщение проверки данных.|
| [input_title](/cells/ru/python-net/aspose.cells/validation/input_title) | Представляет заголовок диалогового окна ввода данных для проверки данных.|
| [error_message](/cells/ru/python-net/aspose.cells/validation/error_message) | Представляет сообщение об ошибке проверки данных.|
| [error_title](/cells/ru/python-net/aspose.cells/validation/error_title) | Представляет заголовок диалогового окна ошибки проверки данных.|
| [show_input](/cells/ru/python-net/aspose.cells/validation/show_input) | Указывает, будет ли отображаться входное сообщение проверки данных всякий раз, когда пользователь выбирает ячейку в диапазоне проверки данных.|
| [show_error](/cells/ru/python-net/aspose.cells/validation/show_error) | Указывает, будет ли отображаться сообщение об ошибке проверки данных всякий раз, когда пользователь вводит недопустимые данные.|
| [ignore_blank](/cells/ru/python-net/aspose.cells/validation/ignore_blank) | Указывает, разрешены ли пустые значения проверкой данных диапазона.|
| [formula1](/cells/ru/python-net/aspose.cells/validation/formula1) | Представляет значение или выражение, связанное с проверкой данных.|
| [formula2](/cells/ru/python-net/aspose.cells/validation/formula2) | Представляет значение или выражение, связанное с проверкой данных.|
| [value1](/cells/ru/python-net/aspose.cells/validation/value1) | Представляет первое значение, связанное с проверкой данных.|
| [value2](/cells/ru/python-net/aspose.cells/validation/value2) | Представляет второе значение, связанное с проверкой данных.|
| [in_cell_drop_down](/cells/ru/python-net/aspose.cells/validation/in_cell_drop_down) | Указывает, отображает ли проверка данных раскрывающийся список, содержащий допустимые значения.|
| [areas](/cells/ru/python-net/aspose.cells/validation/areas) | Получает все [CellArea](/cells/ru/python-net/aspose.cells/cellarea), содержащие параметры проверки данных.|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Получает значение или выражение, связанное с этой проверкой.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/ru/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.|
| [get_formula2(is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Получает значение или выражение, связанное с этой проверкой.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/ru/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.|
| [add_area(cell_area)](/cells/ru/python-net/aspose.cells/validation/add_area/#CellArea) | Применяет проверку к области.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/ru/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | Применяет проверку к области.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | Задает значение или выражение, связанное с этой проверкой.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | Задает значение или выражение, связанное с этой проверкой.|
| [get_list_value(row, column)](/cells/ru/python-net/aspose.cells/validation/get_list_value/#int-int) |Получите значение для списка проверки для указанной ячейки.|
| [add_areas(areas, check_intersection, check_edge)](/cells/ru/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Применяет проверку к заданным областям.|
| [remove_area(cell_area)](/cells/ru/python-net/aspose.cells/validation/remove_area/#CellArea) | Удалите параметры проверки в диапазоне.|
| [remove_areas(areas)](/cells/ru/python-net/aspose.cells/validation/remove_areas/#list) | Удаляет эту проверку из заданных областей.|
| [remove_a_cell(row, column)](/cells/ru/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Удалите настройки проверки в ячейке.|
| [copy(source, copy_option)](/cells/ru/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | Скопируйте подтверждение.|



###  Пример

```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [CellArea](/cells/ru/python-net/aspose.cells/cellarea)
