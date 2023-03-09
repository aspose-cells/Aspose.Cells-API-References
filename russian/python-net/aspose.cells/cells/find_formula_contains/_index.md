---
title: find_formula_contains метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 310
url: /ru/python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---
##  find_formula_contains(formula, previous_cell) {#str-Cell}
Находит ячейку с формулой, содержащей введенную строку.


###  Возвращает

Cell объект.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула для поиска.|
| previous_cell | [Cell](/cells/ru/python-net/aspose.cells/cell) |Предыдущая ячейка с той же формулой. Для этого параметра можно установить значение null, если поиск выполняется с самого начала.|
###  Примечания

Возвращает null (ничего), если ячейка не найдена.
 ПРИМЕЧАНИЕ. Этот элемент устарел.
используйте метод Cells.Find(object,Cell,FindOptions) с LookInType как LookInType.OnlyFormulas
 и LookAtType как LookAtType.Contains.
 Этот участник будет удален через 12 месяцев с ноября 2018 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
