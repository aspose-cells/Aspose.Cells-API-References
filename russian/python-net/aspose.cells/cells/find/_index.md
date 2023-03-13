---
title: find метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 290
url: /ru/python-net/aspose.cells/cells/find/
is_root: false
---
##  find(what, previous_cell) {#any-Cell}
Находит ячейку, содержащую входной объект.


###  Возвращает

Cell объект.


```python
def find(self, what, previous_cell):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| what | any | Объект для поиска.<br/> Тип должен быть int, double, DateTime, string, bool.|
| previous_cell | [Cell](/cells/ru/python-net/aspose.cells/cell) | Предыдущая ячейка с тем же объектом.<br/> Этот параметр может быть установлен равным нулю, если поиск выполняется с самого начала.|
###  Примечания

Возвращает null (ничего), если ячейка не найдена.

##  find(what, previous_cell, find_options) {#any-Cell-FindOptions}

Находит ячейку, содержащую входной объект.


###  Возвращает

Cell объект.


```python
def find(self, what, previous_cell, find_options):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| what | any | Объект для поиска.<br/> Тип должен быть int, double, DateTime, string, bool.|
| previous_cell | [Cell](/cells/ru/python-net/aspose.cells/cell) | Предыдущая ячейка с тем же объектом.<br/> Этот параметр может быть установлен равным нулю, если поиск выполняется с самого начала.|
| find_options | [FindOptions](/cells/ru/python-net/aspose.cells/findoptions) | Найти варианты|
###  Примечания

Возвращает null (ничего), если ячейка не найдена.


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
