---
title: refresh_dynamic_array_formulas метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 270
url: /ru/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/
is_root: false
---
##  refresh_dynamic_array_formulas(calculate) {#bool}
Обновляет формулы динамического массива (перетекает в новый диапазон соседних ячеек в соответствии с текущими данными)
Другие формулы в рабочей книге не будут вычисляться рекурсивно, даже если они использовались формулами динамического массива.



```python
def refresh_dynamic_array_formulas(self, calculate):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| calculate | bool | Вычисляет ли и обновляет значения ячеек для этих формул динамического массива|


##  refresh_dynamic_array_formulas(calculate, copts) {#bool-CalculationOptions}
Обновляет формулы динамического массива (перетекает в новый диапазон соседних ячеек в соответствии с текущими данными)



```python
def refresh_dynamic_array_formulas(self, calculate, copts):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| calculate | bool | Вычисляет ли и обновляет значения ячеек для этих формул динамического массива|
| copts | [CalculationOptions](/cells/ru/python-net/aspose.cells/calculationoptions) | Варианты расчета формул|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
