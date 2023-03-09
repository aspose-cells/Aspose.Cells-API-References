---
title: calculate_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
Вычисляет формулу.


###  Возвращает

Результат расчетной формулы.


```python
def calculate_formula(self, formula):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула для расчета.|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
Вычисляет формулу.


###  Возвращает

Результат расчетной формулы.


```python
def calculate_formula(self, formula, opts):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| formula | str | Формула для расчета.|
| opts | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета формулы|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
Вычисляет все формулы на этом листе.



```python
def calculate_formula(self, options, recursive):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| options | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета|
| recursive | bool | True означает, что ячейки рабочего листа зависят от ячеек других рабочих листов,<br/>зависимые ячейки на других листах также будут рассчитаны.<br/> False означает, что все формулы на листе были рассчитаны и значения верны.|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
Вычисляет все формулы на этом листе.



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| recursive | bool | True означает, что ячейки рабочего листа зависят от ячеек других рабочих листов,<br/>зависимые ячейки на других листах также будут рассчитаны.<br/> False означает, что все формулы на листе были рассчитаны и значения верны.|
| ignore_error | bool | Указывает, если скрыть ошибку при вычислении формул.<br/> Ошибка может заключаться в неподдерживаемых функциях, внешних ссылках и т.д.|
| custom_function | [ICustomFunction](/cells/ru/python-net/aspose.cells/icustomfunction) | Функции вычисления пользовательских формул для расширения механизма вычислений.|
###  Примечания

ПРИМЕЧАНИЕ. Этот элемент устарел.
пожалуйста, используйте метод CalculateFormula(CalculationOptions, bool).
 Этот метод будет удален через 12 месяцев, начиная с августа 2020 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
