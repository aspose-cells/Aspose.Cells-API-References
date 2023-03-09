---
title: characters метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Возвращает объект символов, представляющий диапазон characters в тексте ячейки.


###  Возвращает

Объекты персонажей.


```python
def characters(self, start_index, length):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| start_index | int | Индекс начала персонажа.|
| length | int | Количество символов.|
###  Примечания

Этот метод работает только с ячейками со строковыми значениями.
###  Примеры


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
