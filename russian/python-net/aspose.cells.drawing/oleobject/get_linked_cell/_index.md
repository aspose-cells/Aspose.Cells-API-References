---
title: get_linked_cell метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells.drawing/oleobject/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Получает диапазон, связанный со значением элемента управления.


###  Возвращает

Диапазон, связанный со значением элемента управления.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| is_r1c1 | bool | Нужно ли форматировать формулу как R1C1.|
| is_local | bool | Нужно ли форматировать формулу по локали.|

###  Пример

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject)
