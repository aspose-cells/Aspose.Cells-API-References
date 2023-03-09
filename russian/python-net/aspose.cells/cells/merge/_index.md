---
title: merge метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 790
url: /ru/python-net/aspose.cells/cells/merge/
is_root: false
---
##  merge(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Объединяет указанный диапазон ячеек в одну ячейку.



```python
def merge(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| first_row | int | Первая строка этого диапазона (с нуля)|
| first_column | int | Первый столбец этого диапазона (с нуля)|
| total_rows | int | Количество рядов (на основе одного)|
| total_columns | int | Количество столбцов (на основе одного)|
###  Примечания

Ссылка на объединенную ячейку через адрес верхней левой ячейки в диапазоне.

##  merge(first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}

Объединяет указанный диапазон ячеек в одну ячейку.



```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| first_row | int | Первая строка этого диапазона (с нуля)|
| first_column | int | Первый столбец этого диапазона (с нуля)|
| total_rows | int | Количество рядов (на основе одного)|
| total_columns | int | Количество столбцов (на основе одного)|
| merge_conflict | bool | Объединить конфликтующие объединенные диапазоны.|
###  Примечания

Ссылка на объединенную ячейку через адрес верхней левой ячейки в диапазоне.
Если mergeConflict имеет значение true и объединенный диапазон конфликтует с другими объединенными ячейками,
другие объединенные ячейки будут автоматически удалены.

##  merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
Объединяет указанный диапазон ячеек в одну ячейку.



```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| first_row | int | Первая строка этого диапазона (с нуля)|
| first_column | int | Первый столбец этого диапазона (с нуля)|
| total_rows | int | Количество рядов (на основе одного)|
| total_columns | int | Количество столбцов (на основе одного)|
| check_conflict | bool | Указывает, пересекает ли проверка объединенных ячеек другие объединенные ячейки.|
| merge_conflict | bool | Объединить конфликтующие объединенные диапазоны.|
###  Примечания

Ссылка на объединенную ячейку через адрес верхней левой ячейки в диапазоне.
Если mergeConflict имеет значение true и объединенный диапазон конфликтует с другими объединенными ячейками,
другие объединенные ячейки будут автоматически удалены.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
