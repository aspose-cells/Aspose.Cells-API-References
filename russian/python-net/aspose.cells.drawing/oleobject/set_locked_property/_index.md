---
title: set_locked_property метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 200
url: /ru/python-net/aspose.cells.drawing/oleobject/set_locked_property/
is_root: false
---
##  set_locked_property(type, value) {#ShapeLockType-bool}
Установите заблокированное свойство.



```python
def set_locked_property(self, type, value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ShapeLockType](/cells/ru/python-net/aspose.cells.drawing/shapelocktype) | Запертый тип.|
| value | bool | Стоимость имущества.|

###  Пример

```python
from aspose.cells.drawing import ShapeLockType

shape.set_locked_property(ShapeLockType.ADJUST_HANDLES, True)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject)
