---
title: calculated_value недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value недвижимость

Получает или задает вычисленное значение для этой функции.

###  Примечания

Пользователь должен установить это свойство в своем пользовательском механизме расчета для тех функций, которые поддерживает этот механизм.
и установленное значение будет возвращено при получении этого свойства позже.
Установленное значение может быть любым значением тех объектов, которые могут быть установлены на Cell(Cell.Value).
И это также может быть массив таких значений или Range, Name, ReferredArea.
Получение этого свойства перед настройкой приведет к тому, что функция будет вычислена механизмом вычислений по умолчанию Aspose.Cells, и вычисленное значение будет возвращено.
###  Определение:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [CalculationData](/cells/ru/python-net/aspose.cells/calculationdata)
