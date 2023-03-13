---
title: calc_stack_size недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size недвижимость

Указывает размер стека для рекурсивного вычисления ячеек.
Большое значение этого размера даст лучшую производительность, когда необходимо рекурсивно вычислить большое количество ячеек.
С другой стороны, большее значение повысит риск StackOverflowException.
Если пользователь получает StackOverflowException при вычислении формул, это значение следует уменьшить.

###  Примечания

ПРИМЕЧАНИЕ. Этот элемент устарел. Вместо этого используйте CalculationOptions
с указанным CalcStackSize при вычислении формул.
 Это свойство будет удалено через 12 месяцев, начиная с февраля 2022 года.
Aspose приносит извинения за возможные неудобства.
###  Определение:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [WorkbookSettings](/cells/ru/python-net/aspose.cells/workbooksettings)
