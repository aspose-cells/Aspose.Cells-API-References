---
title: calc_stack_size propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size propiedad

Especifica el tamaño de pila para calcular celdas recursivamente.
El valor grande para este tamaño brindará un mejor rendimiento cuando haya muchas celdas que se deban calcular recursivamente.
Por otro lado, un valor mayor aumentará el riesgo de StackOverflowException.
Si el usuario obtiene StackOverflowException al calcular fórmulas, este valor debe reducirse.

###  Observaciones

NOTA: Este miembro ahora está obsoleto. En su lugar, utilice CalculationOptions
con el CalcStackSize especificado al calcular fórmulas.
 Esta propiedad se eliminará 12 meses después desde febrero de 2022.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.
###  Definición:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [WorkbookSettings](/cells/es/python-net/aspose.cells/workbooksettings)
