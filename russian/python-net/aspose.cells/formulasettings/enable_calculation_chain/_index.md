---
title: enable_calculation_chain недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain недвижимость

Включить ли цепочку вычислений для формул. Значение по умолчанию — ложь.

###  Примечания

Когда в рабочей книге много формул, и пользователю необходимо многократно их вычислять
при изменении лишь небольшой их части может быть полезно для производительности включить цепочку вычислений.
С другой стороны, если цепочка включена, поддержание модели цепочки требует дополнительной памяти,
и это также требует немного больше процессорного времени для некоторых других операций, таких как изменение значения ячейки или формул.
После изменения этого свойства с false на true цепочка вычислений будет проанализирована и построена
во время первого расчета для рабочей книги, поэтому необходимое время для первого расчета
может быть больше, чем обычный расчет без цепочки.
###  Определение:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [FormulaSettings](/cells/ru/python-net/aspose.cells/formulasettings)
