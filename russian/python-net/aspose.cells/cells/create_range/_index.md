---
title: create_range метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 190
url: /ru/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из адреса диапазона.


###  Возвращает

Объект [Range](/cells/ru/python-net/aspose.cells/range)


```python
def create_range(self, address):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| address | str | Адрес диапазона.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из диапазона ячеек.


###  Возвращает

Объект [Range](/cells/ru/python-net/aspose.cells/range)


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_cell | str | Имя верхней левой ячейки.|
| lower_right_cell | str | Имя нижней правой ячейки.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из строк ячеек или столбцов ячеек.


###  Возвращает

Объект [Range](/cells/ru/python-net/aspose.cells/range).


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| first_index | int | Индекс первой строки или индекс первого столбца, отсчитываемый от нуля.|
| number | int | Общее количество строк или столбцов, по одному.|
| is_vertical | bool | True — диапазон, созданный из столбцов ячеек. False — диапазон создан из строк ячеек.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Создает объект [Range](/cells/ru/python-net/aspose.cells/range) из диапазона ячеек.


###  Возвращает

Объект [Range](/cells/ru/python-net/aspose.cells/range)


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| first_row | int | Первая строка этого диапазона|
| first_column | int | Первый столбец этого диапазона|
| total_rows | int | Количество рядов|
| total_columns | int | Число столбцов|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
