---
title: set_dynamic_array_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 310
url: /ru/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.


###  Возвращает

диапазон, в который должна попасть формула.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| array_formula | str | выражение формулы|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | варианты разбора формулы.<br/> Параметр «Разбор» будет игнорироваться, и формула всегда будет анализироваться немедленно.|
| calculate_value | bool | вычислить ли эту формулу динамического массива для тех ячеек в разлитом диапазоне.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.


###  Возвращает

диапазон, в который должна попасть формула.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| array_formula | str | выражение формулы|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | варианты разбора формулы.<br/> Параметр «Разбор» будет игнорироваться, и формула всегда будет анализироваться немедленно.|
| values | list |значения для тех ячеек с заданной формулой динамического массива|
| calculate_range | bool | Вычислите ли разбросанный диапазон для этой формулы динамического массива.<br/>Если параметр "values" не нулевой и этот флаг ложный,<br/>тогда высота разлитого диапазона будет значениями. Длина и ширина будут значениями [0]. Длина.|
| calculate_value | bool | вычислить ли эту формулу динамического массива для тех ячеек в пролитом диапазоне, когда «значения» равны нулю<br/> или соответствующий элемент в «значениях» для одной ячейки равен нулю.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Задает формулу динамического массива и по возможности распространяет формулу на соседние ячейки.


###  Возвращает

диапазон, в который должна попасть формула.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| array_formula | str | выражение формулы|
| options | [FormulaParseOptions](/cells/ru/python-net/aspose.cells/formulaparseoptions) | варианты разбора формулы.<br/> Параметр «Разбор» будет игнорироваться, и формула всегда будет анализироваться немедленно.|
| values | list |значения для тех ячеек с заданной формулой динамического массива|
| calculate_range | bool | Вычислите ли разбросанный диапазон для этой формулы динамического массива.<br/>Если параметр "values" не нулевой и этот флаг ложный,<br/>тогда высота разлитого диапазона будет значениями. Длина и ширина будут значениями [0]. Длина.|
| calculate_value | bool | вычислить ли эту формулу динамического массива для тех ячеек в пролитом диапазоне, когда «значения» равны нулю<br/> или соответствующий элемент в «значениях» для одной ячейки равен нулю.|
| copts | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета формулы.<br/> Обычно из соображений производительности свойство [CalculationOptions.recursive](/cells/ru/python-net/aspose.cells/calculationoptions#recursive) должно иметь значение false.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
