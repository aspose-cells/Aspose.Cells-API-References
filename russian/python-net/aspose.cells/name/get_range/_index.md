---
title: get_range метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/name/get_range/
is_root: false
---
##  get_range() {#}
Получает диапазон, если это имя относится к диапазону.


###  Возвращает

Диапазон.


```python
def get_range(self):
    ...
```




##  get_range(recalculate) {#bool}
Получает диапазон, если это имя относится к диапазону


###  Возвращает

Диапазон.


```python
def get_range(self, recalculate):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| recalculate | bool | пересчитать ли его, если это имя было вычислено до этого вызова.|


##  get_range(sheet_index, row, column) {#int-int-int}
Получает диапазон, если это имя относится к диапазону.
Если ссылка на это имя не является абсолютной, диапазон может быть разным для разных ячеек.


###  Возвращает

Диапазон.


```python
def get_range(self, sheet_index, row, column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| sheet_index | int |Соответствующий индекс листа.|
| row | int | Соответствующий индекс строки.|
| column | int | Соответствующий индекс столбца|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Name](/cells/ru/python-net/aspose.cells/name)
