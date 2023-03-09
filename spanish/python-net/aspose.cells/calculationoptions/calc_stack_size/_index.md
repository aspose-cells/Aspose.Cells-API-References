---
title: calc_stack_size propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size propiedad

Especifica el tamaño de pila para calcular celdas recursivamente.

###  Observaciones

Cuando hay una gran cantidad de celdas que deben calcularse recursivamente en el árbol de dependencia,
StackOverflowException puede producirse en el proceso de cálculo.
Si es así, el usuario debe especificar un valor menor para esta propiedad.
Para tal situación, el usuario debe determinar el valor adecuado para esta propiedad de acuerdo con las fórmulas y los datos reales.
Un valor demasiado pequeño puede causar una degradación del rendimiento para el cálculo de la fórmula.
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
* clase [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions)
