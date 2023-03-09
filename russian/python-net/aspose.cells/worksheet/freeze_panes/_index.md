---
title: freeze_panes метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 120
url: /ru/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
Замораживает панели в указанной ячейке листа.



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| cell_name | str | Cell имя.|
| freezed_rows | int | Количество видимых строк в верхней панели, не более индекса строки.|
| freezed_columns | int | Количество видимых столбцов в левой панели, не более индекса столбца.|
###  Примечания

Индекс строки и индекс столбца не могут быть равны нулю.
также не могут быть все равны нулю.

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
Замораживает панели в указанной ячейке листа.



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row | int | Индекс строки.|
| column | int | Индекс столбца.|
| freezed_rows | int | Количество видимых строк в верхней панели, не более индекса строки.|
| freezed_columns | int | Количество видимых столбцов в левой панели, не более индекса столбца.|
###  Примечания

Индекс строки и индекс столбца не могут быть равны нулю.
также не могут быть все равны нулю.


Первые два параметра определяют фиксированную позицию, а последние два параметра определяют фиксированную область на левой верхней панели.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
