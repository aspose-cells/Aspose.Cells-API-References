---
title: calculated_value propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value propiedad

Obtiene o establece el valor calculado para esta función.

###  Observaciones

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que admite el motor,
el valor establecido se devolverá al obtener esta propiedad más adelante.
El valor establecido puede ser cualquier valor de esos objetos que se pueden establecer en Cell (Cell. Valor).
Y también puede ser una matriz de este tipo de valores, o un Rango, Nombre, Área de referencia.
Obtener esta propiedad antes de la configuración hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y se devolverá el valor calculado.
###  Definición:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [CalculationData](/cells/es/python-net/aspose.cells/calculationdata)
