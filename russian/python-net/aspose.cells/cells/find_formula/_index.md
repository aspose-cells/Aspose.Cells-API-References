---
title: find_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 300
url: /ru/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
Находит ячейку с входной строкой.


###  Возвращает

Cell объект.


```python
def find_formula(self, formula, previous_cell):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула для поиска.|
| previous_cell | [Cell](/cells/ru/python-net/aspose.cells/cell) |Предыдущая ячейка с той же формулой. Этот параметр может быть установлен равным нулю, если поиск выполняется с самого начала.|
###  Примечания

Возвращает null (ничего), если ячейка не найдена.
 ПРИМЕЧАНИЕ. Этот элемент устарел. Вместо,
используйте метод Cells.Find(object,Cell,FindOptions) с LookInType как LookInType.OnlyFormulas
 и LookAtType как LookAtType.EntireContent.
 Этот участник будет удален через 12 месяцев с ноября 2018 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
