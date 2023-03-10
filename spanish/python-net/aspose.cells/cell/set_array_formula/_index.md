---
title: set_array_formula método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Establece una fórmula de matriz (fórmula de matriz heredada ingresada mediante CTRL+MAYÚS+ENTRAR en MS Excel) en un rango de celdas.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | Fórmula matricial.|
| row_number | int |Número de filas para completar el resultado de la fórmula de matriz.|
| column_number | int | Número de columnas para completar el resultado de la fórmula de matriz.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Establece una fórmula de matriz en un rango de celdas.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | Fórmula matricial.|
| row_number | int |Número de filas para completar el resultado de la fórmula de matriz.|
| column_number | int | Número de columnas para completar el resultado de la fórmula de matriz.|
| options | [FormulaParseOptions](/cells/es/python-net/aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Establece una fórmula de matriz en un rango de celdas.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | Fórmula matricial.|
| row_number | int |Número de filas para completar el resultado de la fórmula de matriz.|
| column_number | int | Número de columnas para completar el resultado de la fórmula de matriz.|
| is_r1c1 | bool | si la fórmula es la fórmula R1C1|
| is_local | bool | si la fórmula tiene formato local|
###  Observaciones

NOTA: Esta clase ahora está obsoleta. En cambio,
utilice Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
Esta propiedad se eliminará 12 meses después desde diciembre de 2019.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Establece una fórmula de matriz en un rango de celdas.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| array_formula | str | Fórmula matricial.|
| row_number | int |Número de filas para completar el resultado de la fórmula de matriz.|
| column_number | int | Número de columnas para completar el resultado de la fórmula de matriz.|
| options | [FormulaParseOptions](/cells/es/python-net/aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula.|
| values | list | valores para esas celdas con fórmula de matriz dada|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
