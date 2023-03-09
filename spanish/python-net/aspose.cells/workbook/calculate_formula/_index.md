---
title: calculate_formula método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Calcula el resultado de fórmulas.



```python
def calculate_formula(self):
    ...
```


###  Observaciones

Para todas las fórmulas admitidas, consulte la lista en https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

##  calculate_formula(ignore_error) {#bool}

Calcula el resultado de fórmulas.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| ignore_error | bool | Indica si se oculta el error en el cálculo de fórmulas.|


##  calculate_formula(options) {#CalculationOptions}
Cálculo de fórmulas en este libro de trabajo.



```python
def calculate_formula(self, options):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| options | [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions) | Opciones de cálculo|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Calcula el resultado de fórmulas.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| ignore_error | bool | Indica si se oculta el error en el cálculo de fórmulas.|
| custom_function | [ICustomFunction](/cells/es/python-net/aspose.cells/icustomfunction) | Las funciones de cálculo de fórmula personalizada para ampliar el motor de cálculo.|
###  Observaciones

NOTA: Este miembro ahora está obsoleto.
utilice el método CalculateFormula (CalculationOptions).
 Este método se eliminará 12 meses después desde agosto de 2020.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
