---
title: calculate метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/cell/calculate/
is_root: false
---
##  calculate(options) {#CalculationOptions}
Вычисляет формулу ячейки.



```python
def calculate(self, options):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| options | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета|


##  calculate(ignore_error, custom_function) {#bool-ICustomFunction}
Вычисляет формулу ячейки.



```python
def calculate(self, ignore_error, custom_function):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| ignore_error | bool | Указывает, если скрыть ошибку при вычислении формул.<br/> Ошибка может быть в неподдерживаемой функции, внешних ссылках и т.п.|
| custom_function | [ICustomFunction](/cells/ru/python-net/aspose.cells/icustomfunction) | Функции вычисления пользовательских формул для расширения механизма вычислений.|
###  Примечания

ПРИМЕЧАНИЕ. Этот элемент устарел. Вместо,
пожалуйста, используйте метод Calculate(CalculationOptions).
 Этот метод будет удален через 12 месяцев, начиная с августа 2020 года.
Aspose приносит извинения за возможные неудобства.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
