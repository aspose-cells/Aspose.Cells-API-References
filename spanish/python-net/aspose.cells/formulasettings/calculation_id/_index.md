---
title: calculation_id propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id propiedad

Especifica la versión del motor de cálculo utilizado para calcular valores en el libro.

###  Observaciones

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante
para que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante.
En el caso de ms excel, si el valor de esta propiedad es menor que el identificador del motor de recálculo asociado
con la aplicación que abre el archivo resultante, la aplicación volverá a calcular los resultados de todas las fórmulas
en este libro inmediatamente después de cargar el archivo.
Para tener en cuenta el rendimiento de la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de forma automática,
independientemente del valor que se haya establecido para esta propiedad.
###  Definición:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [FormulaSettings](/cells/es/python-net/aspose.cells/formulasettings)
