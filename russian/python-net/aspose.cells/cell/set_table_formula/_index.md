---
title: set_table_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 350
url: /ru/python-net/aspose.cells/cell/set_table_formula/
is_root: false
---
##  set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values) {#int-int-str-str-list}
Создайте таблицу данных с двумя переменными для заданного диапазона, начиная с этой ячейки.



```python
def set_table_formula(self, row_number, column_number, row_input_cell, column_input_cell, values):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_number | int |Количество строк для заполнения формулы.|
| column_number | int | Количество столбцов для заполнения формулы.|
| row_input_cell | str | ячейка ввода строки|
| column_input_cell | str | ячейка ввода столбца|
| values | list | значения для ячеек в диапазоне формулы таблицы|


##  set_table_formula(row_number, column_number, input_cell, is_row_input, values) {#int-int-str-bool-list}
Создайте таблицу данных с одной переменной для заданного диапазона, начиная с этой ячейки.



```python
def set_table_formula(self, row_number, column_number, input_cell, is_row_input, values):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_number | int |Количество строк для заполнения формулы.|
| column_number | int | Количество столбцов для заполнения формулы.|
| input_cell | str | входная ячейка|
| is_row_input | bool | Указывает, является ли входная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false).|
| values | list | значения для ячеек в диапазоне формулы таблицы|


##  set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values) {#int-int-int-int-bool-list}
Создайте таблицу данных с одной переменной для заданного диапазона, начиная с этой ячейки.



```python
def set_table_formula(self, row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_number | int |Количество строк для заполнения формулы.|
| column_number | int | Количество столбцов для заполнения формулы.|
| row_index_of_input_cell | int | индекс строки входной ячейки|
| column_index_of_input_cell | int | индекс столбца входной ячейки|
| is_row_input | bool | Указывает, является ли входная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false).|
| values | list | значения для ячеек в диапазоне формулы таблицы|


##  set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values) {#int-int-int-int-int-int-list}
Создайте таблицу данных с двумя переменными для заданного диапазона, начиная с этой ячейки.



```python
def set_table_formula(self, row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_number | int |Количество строк для заполнения формулы.|
| column_number | int | Количество столбцов для заполнения формулы.|
| row_index_of_row_input_cell | int |индекс строки входной ячейки строки|
| column_index_of_row_input_cell | int | индекс столбца ячейки ввода строки|
| row_index_of_column_input_cell | int | индекс строки входной ячейки столбца|
| column_index_of_column_input_cell | int | индекс столбца входной ячейки столбца|
| values | list | значения для ячеек в диапазоне формулы таблицы|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
