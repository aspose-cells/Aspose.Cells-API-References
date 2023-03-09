---
title: calc_stack_size недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size недвижимость

Указывает размер стека для рекурсивного вычисления ячеек.

###  Примечания

Когда в дереве зависимостей необходимо рекурсивно вычислить большое количество ячеек,
StackOverflowException может быть вызвано в процессе вычисления.
Если это так, пользователь должен указать меньшее значение для этого свойства.
В такой ситуации пользователь должен определить правильное значение этого свойства в соответствии с фактическими формулами и данными.
Слишком маленькое значение может привести к снижению производительности при расчете по формуле.
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
* класс [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions)
