---
title: calculate método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/cell/calculate/
is_root: false
---
##  calculate(options) {#CalculationOptions}
Calcula la fórmula de la celda.



```python
def calculate(self, options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| options | [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions) | Opciones de cálculo|


##  calculate(ignore_error, custom_function) {#bool-ICustomFunction}
Calcula la fórmula de la celda.



```python
def calculate(self, ignore_error, custom_function):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| ignore_error | bool | Indica si se oculta el error en el cálculo de fórmulas.<br/> El error puede ser una función no compatible, enlaces externos, etc.|
| custom_function | [ICustomFunction](/cells/es/python-net/aspose.cells/icustomfunction) | Las funciones de cálculo de fórmula personalizada para ampliar el motor de cálculo.|
###  Observaciones

NOTA: Este miembro ahora está obsoleto. En cambio,
utilice el método Calculate (CalculationOptions).
 Este método se eliminará 12 meses después desde agosto de 2020.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
