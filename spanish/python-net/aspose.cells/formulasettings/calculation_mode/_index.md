---
title: calculation_mode propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode propiedad

Obtiene o establece el modo para el cálculo del libro de trabajo en MS Excel.

###  Observaciones

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante
para que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante.
Para tener en cuenta el rendimiento de la aplicación de la mayoría de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente,
independientemente del modo que se haya establecido para esta propiedad.
Si el usuario necesita calcular fórmulas, llame siempre a métodos en diferentes objetos según los requisitos:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/python-net/aspose.cells/cell/calculate), ...etc.
###  Definición:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [CalcModeType](/cells/es/python-net/aspose.cells/calcmodetype)
* clase [FormulaSettings](/cells/es/python-net/aspose.cells/formulasettings)
