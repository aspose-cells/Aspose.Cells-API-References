---
title: pivot_source propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 400
url: /es/python-net/aspose.cells.charts/chart/pivot_source/
is_root: false
---
##  pivot_source propiedad

La fuente son los datos de la tabla dinámica.
Si PivotSource no está vacío, el gráfico es PivotChart.

###  Observaciones

Si la tabla dinámica "PivotTable1" en la hoja de trabajo "Sheet1" en el archivo "Book1.xls".
El pivotSource podría ser "[Book1.xls]Sheet1!PivotTable1" si el gráfico y la tabla dinámica no están en el mismo libro.
Si establece esta propiedad, se perderá la configuración de la fuente de datos anterior.
###  Definición:
```python
@property
def pivot_source(self):
    ...
@pivot_source.setter
def pivot_source(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [Chart](/cells/es/python-net/aspose.cells.charts/chart)
