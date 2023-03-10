---
title: is_param_literal_required propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
##  is_param_literal_required propiedad

Indica si este motor necesita el texto literal del parámetro mientras realiza el cálculo. El valor predeterminado es falso.

###  Observaciones

Si este motor de cálculo personalizado requiere el texto literal del parámetro, se requerirán más pilas para almacenar en caché el texto literal de los parámetros y se puede llamar al método Calculate() de forma recursiva para calcular el valor del parámetro.
Por lo general, el texto literal no es necesario para calcular fórmulas y este método debería devolver falso para la mayoría de las implementaciones para obtener un mejor rendimiento.
###  Definición:
```python
@property
def is_param_literal_required(self):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [AbstractCalculationEngine](/cells/es/python-net/aspose.cells/abstractcalculationengine)
