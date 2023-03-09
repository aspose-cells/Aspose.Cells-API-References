---
title: get_list_value метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Получите значение для списка проверки для указанной ячейки.


###  Возвращает

Значение для создания списка этой проверки для указанной ячейки.
Если список ссылается на диапазон, то возвращаемое значение будет объектом [ReferredArea](/cells/ru/python-net/aspose.cells/referredarea);
В противном случае возвращаемое значение может быть нулевым, объектом[] или простым объектом.


```python
def get_list_value(self, row, column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row | int | Индекс строки.|
| column | int | Индекс столбца.|
###  Примечания

Только для проверки, тип которой — список и которая была применена к данной ячейке,
в противном случае будет возвращено значение null.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [ReferredArea](/cells/ru/python-net/aspose.cells/referredarea)
* класс [Validation](/cells/ru/python-net/aspose.cells/validation)
