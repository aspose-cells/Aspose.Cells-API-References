---
title: set_dynamic_array_formula método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 310
url: /es/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.


###  Devoluciones

el rango en el que debe derramarse la fórmula.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | la expresión de la fórmula|
| options | [FormulaParseOptions](/cells/es/python-net/aspose.cells/formulaparseoptions) | opciones para analizar la fórmula.<br/> La opción "Analizar" se ignorará y la fórmula siempre se analizará inmediatamente|
| calculate_value | bool | si calcula esta fórmula de matriz dinámica para esas celdas en el rango derramado.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.


###  Devoluciones

el rango en el que debe derramarse la fórmula.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | la expresión de la fórmula|
| options | [FormulaParseOptions](/cells/es/python-net/aspose.cells/formulaparseoptions) | opciones para analizar la fórmula.<br/> La opción "Analizar" se ignorará y la fórmula siempre se analizará inmediatamente|
| values | list |valores para esas celdas con fórmula de matriz dinámica dada|
| calculate_range | bool | Si calcula el rango derramado para esta fórmula de matriz dinámica.<br/>Si el parámetro "valores" no es nulo y este indicador es falso,<br/> entonces la altura del rango derramado será valores. La longitud y el ancho serán valores [0]. Longitud.|
| calculate_value | bool | si calcula esta fórmula de matriz dinámica para esas celdas en el rango derramado cuando "valores" es nulo<br/> o el elemento correspondiente en "valores" para una celda es nulo.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.


###  Devoluciones

el rango en el que debe derramarse la fórmula.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | la expresión de la fórmula|
| options | [FormulaParseOptions](/cells/es/python-net/aspose.cells/formulaparseoptions) | opciones para analizar la fórmula.<br/> La opción "Analizar" se ignorará y la fórmula siempre se analizará inmediatamente|
| values | list |valores para esas celdas con fórmula de matriz dinámica dada|
| calculate_range | bool | Si calcula el rango derramado para esta fórmula de matriz dinámica.<br/>Si el parámetro "valores" no es nulo y este indicador es falso,<br/> entonces la altura del rango derramado será valores. La longitud y el ancho serán valores [0]. Longitud.|
| calculate_value | bool | si calcula esta fórmula de matriz dinámica para esas celdas en el rango derramado cuando "valores" es nulo<br/> o el elemento correspondiente en "valores" para una celda es nulo.|
| copts | [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions) | Las opciones para calcular la fórmula.<br/> Por lo general, para tener en cuenta el rendimiento, la propiedad [CalculationOptions.recursive](/cells/es/python-net/aspose.cells/calculationoptions#recursive) debería ser falsa.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
