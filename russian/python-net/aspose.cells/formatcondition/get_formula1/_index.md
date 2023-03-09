---
title: get_formula1 метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/formatcondition/get_formula1/
is_root: false
---
##  get_formula1(is_r1c1, is_local) {#bool-bool}
Получает значение или выражение, связанное с этим условием формата.


###  Возвращает

Значение или выражение, связанное с этим условием формата.


```python
def get_formula1(self, is_r1c1, is_local):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| is_r1c1 | bool | Нужно ли форматировать формулу как R1C1.|
| is_local | bool | Нужно ли форматировать формулу по локали.|


##  get_formula1(row, column) {#int-int}
Получает формулу условного форматирования ячейки.


###  Возвращает

Формула.


```python
def get_formula1(self, row, column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row | int | Индекс строки.|
| column | int | Индекс столбца.|


##  get_formula1(is_r1c1, is_local, row, column) {#bool-bool-int-int}
Получает значение или выражение условного форматирования ячейки.


###  Возвращает

Значение или выражение, связанное с условным форматированием ячейки.


```python
def get_formula1(self, is_r1c1, is_local, row, column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| is_r1c1 | bool | Нужно ли форматировать формулу как R1C1.|
| is_local | bool | Нужно ли форматировать формулу по локали.|
| row | int | Индекс строки.|
| column | int | Индекс столбца.|
###  Примечания

Данная ячейка должна содержаться в этом условном форматировании, иначе будет возвращено значение null.


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [FormatCondition](/cells/ru/python-net/aspose.cells/formatcondition)
