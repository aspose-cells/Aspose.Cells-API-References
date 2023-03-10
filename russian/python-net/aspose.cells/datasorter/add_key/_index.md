---
title: add_key метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/datasorter/add_key/
is_root: false
---
##  add_key(key, order) {#int-SortOrder}
Добавляет отсортированный индекс столбца и порядок сортировки.



```python
def add_key(self, key, order):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| key | int | Индекс отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...)|
| order | [SortOrder](/cells/ru/python-net/aspose.cells/sortorder) | Порядок сортировки|


##  add_key(key, order, custom_list) {#int-SortOrder-str}
Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.



```python
def add_key(self, key, order, custom_list):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| key | int | Индекс отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...)|
| order | [SortOrder](/cells/ru/python-net/aspose.cells/sortorder) | Порядок сортировки.|
| custom_list | str | Пользовательский список сортировки.|


##  add_key(key, order, custom_list) {#int-SortOrder-list}
Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.



```python
def add_key(self, key, order, custom_list):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| key | int | Индекс отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...)|
| order | [SortOrder](/cells/ru/python-net/aspose.cells/sortorder) | Порядок сортировки.|
| custom_list | list | Пользовательский список сортировки.|


##  add_key(key, type, order, custom_list) {#int-SortOnType-SortOrder-any}
Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.



```python
def add_key(self, key, type, order, custom_list):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| key | int | Индекс отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...)|
| type | [SortOnType](/cells/ru/python-net/aspose.cells/sortontype) | Тип отсортированного значения.|
| order | [SortOrder](/cells/ru/python-net/aspose.cells/sortorder) | Порядок сортировки.|
| custom_list | any | Пользовательский список сортировки.|
###  Примечания

Если тип — SortOnType.CellColor или SortOnType.FontColor, customList — это Color.


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [DataSorter](/cells/ru/python-net/aspose.cells/datasorter)
