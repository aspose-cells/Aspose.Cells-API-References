---
title: enable_calculation_chain propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain propiedad

Si habilita la cadena de cálculo para fórmulas. El valor predeterminado es falso.

###  Observaciones

Cuando hay muchas fórmulas en el libro de trabajo y el usuario necesita calcularlas repetidamente
modificando solo una pequeña parte de ellos, puede ser útil para el rendimiento habilitar la cadena de cálculo.
Por otro lado, si la cadena está habilitada, mantener el modelo de cadena requiere memoria adicional,
y también requiere un poco más de tiempo de CPU para algunas otras operaciones, como cambiar el valor de la celda o las fórmulas.
Después de cambiar esta propiedad de falso a verdadero, la cadena de cálculo será analizada y construida.
en el momento del primer cálculo del libro de trabajo, por lo que el tiempo requerido para el primer cálculo
puede ser más que un cálculo normal sin cadena.
###  Definición:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [FormulaSettings](/cells/es/python-net/aspose.cells/formulasettings)
