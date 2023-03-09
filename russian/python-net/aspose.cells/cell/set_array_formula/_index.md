---
title: set_array_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 290
url: /ru/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Задает формулу массива (устаревшая формула массива, введенная с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| array_formula | str | Формула массива.|
| row_number | int |Количество строк для заполнения результата формулы массива.|
| column_number | int | Количество столбцов для заполнения результата формулы массива.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Задает формулу массива для диапазона ячеек.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| array_formula | str | Формула массива.|
| row_number | int |Количество строк для заполнения результата формулы массива.|
| column_number | int | Количество столбцов для заполнения результата формулы массива.|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | Варианты разбора формулы.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Задает формулу массива для диапазона ячеек.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| array_formula | str | Формула массива.|
| row_number | int |Количество строк для заполнения результата формулы массива.|
| column_number | int | Количество столбцов для заполнения результата формулы массива.|
| is_r1c1 | bool | является ли формула формулой R1C1|
| is_local | bool | отформатирована ли формула в локали|
###  Примечания

ПРИМЕЧАНИЕ. Этот класс устарел.
пожалуйста, используйте Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года.
Aspose приносит извинения за возможные неудобства.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Задает формулу массива для диапазона ячеек.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| array_formula | str | Формула массива.|
| row_number | int |Количество строк для заполнения результата формулы массива.|
| column_number | int | Количество столбцов для заполнения результата формулы массива.|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | Варианты разбора формулы.|
| values | list | значения для тех ячеек с заданной формулой массива|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
