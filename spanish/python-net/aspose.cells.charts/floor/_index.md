---
title: Floor clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 160
url: /es/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor clase
Encapsula el objeto que representa el suelo de un gráfico 3D.



**Herencia:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/es/python-net/aspose.cells.drawing/area)



El tipo Floor expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [background_color](/cells/es/python-net/aspose.cells.charts/floor/background_color) | Obtiene o establece el Color de fondo del [Area](/cells/es/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/es/python-net/aspose.cells.charts/floor/foreground_color) | Obtiene o establece el Color de primer plano.|
| [formatting](/cells/es/python-net/aspose.cells.charts/floor/formatting) | Representa el formato del área.|
| [invert_if_negative](/cells/es/python-net/aspose.cells.charts/floor/invert_if_negative) | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo,<br/> se intercambiarán el color de primer plano y el color de fondo.|
| [fill_format](/cells/es/python-net/aspose.cells.charts/floor/fill_format) | Representa un objeto [Area.fill_format](/cells/es/python-net/aspose.cells.drawing/area#fill_format) que contiene propiedades de formato de relleno para el gráfico o la forma especificados.|
| [transparency](/cells/es/python-net/aspose.cells.charts/floor/transparency) | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente).|
| [border](/cells/es/python-net/aspose.cells.charts/floor/border) | Obtiene o establece el borde [Line](/cells/es/python-net/aspose.cells.drawing/line).|



###  Ejemplo

```python
from aspose.cells import License, Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientPresetType, GradientStyleType
from aspose.pydrawing import Color

# Instantiate the License class
license = License()
# Pass only the name of the license file embedded in the assembly
license.set_license("Aspose.Cells.lic")
# Instantiate the workbook object
workbook = Workbook()
# Get cells collection
cells = workbook.worksheets[0].cells
# Put values in cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
cells.get("A3").put_value(3)
# get charts colletion
charts = workbook.worksheets[0].charts
# add a new chart
index = charts.add(ChartType.COLUMN_3D_STACKED, 5, 0, 15, 5)
# get the newly added chart
chart = charts[index]
# set charts nseries
chart.n_series.add("A1:A3", True)
# Show data labels
chart.n_series[0].data_labels.show_value = True
# Get chart's floor
floor = chart.floor
# set floor's border as red
floor.border.color = Color.red
# set fill format
floor.fill_format.set_preset_color_gradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2)
# save the file
workbook.save(r"dest.xls")

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [Area](/cells/es/python-net/aspose.cells.drawing/area)
* clase [Floor](/cells/es/python-net/aspose.cells.charts/floor)
* clase [Line](/cells/es/python-net/aspose.cells.drawing/line)
