---
title: set_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 320
url: /ru/python-net/aspose.cells/cell/set_formula/
is_root: false
---
##  set_formula(formula, value) {#str-any}
Установите формулу и значение формулы.



```python
def set_formula(self, formula, value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула.|
| value | any | Значение формулы.|


##  set_formula(formula, options, value) {#str-FormulaParseOptions-any}
Установите формулу и значение формулы.



```python
def set_formula(self, formula, options, value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула.|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | Варианты разбора формулы.|
| value | any | Значение формулы.|


##  set_formula(formula, is_r1c1, is_local, value) {#str-bool-bool-any}
Установите формулу и значение формулы.



```python
def set_formula(self, formula, is_r1c1, is_local, value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула.|
| is_r1c1 | bool | Является ли формула формулой R1C1.|
| is_local | bool | Отформатирована ли формула в языковом стандарте.|
| value | any | Значение формулы.|
###  Примечания

ПРИМЕЧАНИЕ. Этот класс устарел. Вместо,
используйте Cell.SetFormula(строка,FormulaParseOptions,объект).
Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
