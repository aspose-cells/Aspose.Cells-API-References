---
title: calculate_formula метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Вычисляет результат формул.



```python
def calculate_formula(self):
    ...
```


###  Примечания

Все поддерживаемые формулы см. в списке по адресу https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions.

##  calculate_formula(ignore_error) {#bool}

Вычисляет результат формул.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| ignore_error | bool | Указывает, если скрыть ошибку при вычислении формул.|


##  calculate_formula(options) {#CalculationOptions}
Расчетные формулы в этой рабочей тетради.



```python
def calculate_formula(self, options):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| options | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Вычисляет результат формул.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| ignore_error | bool | Указывает, если скрыть ошибку при вычислении формул.|
| custom_function | [ICustomFunction](/cells/ru/python-net/aspose.cells/icustomfunction) | Функции вычисления пользовательских формул для расширения механизма вычислений.|
###  Примечания

ПРИМЕЧАНИЕ. Этот элемент устарел.
пожалуйста, используйте метод CalculateFormula(CalculationOptions).
 Этот метод будет удален через 12 месяцев, начиная с августа 2020 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
