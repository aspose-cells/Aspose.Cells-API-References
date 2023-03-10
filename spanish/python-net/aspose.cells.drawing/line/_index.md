---
title: Line clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line clase
Encapsula el objeto que representa el formato de línea.



El tipo Line expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [compound_type](/cells/es/python-net/aspose.cells.drawing/line/compound_type) | Especifica el tipo de línea compuesta|
| [dash_type](/cells/es/python-net/aspose.cells.drawing/line/dash_type) | Especifica el tipo de línea discontinua|
| [cap_type](/cells/es/python-net/aspose.cells.drawing/line/cap_type) | Especifica las mayúsculas finales.|
| [join_type](/cells/es/python-net/aspose.cells.drawing/line/join_type) | Especifica las tapas de unión.|
| [begin_type](/cells/es/python-net/aspose.cells.drawing/line/begin_type) |Especifica una punta de flecha para el comienzo de una línea.|
| [end_type](/cells/es/python-net/aspose.cells.drawing/line/end_type) | Especifica una punta de flecha para el final de una línea.|
| [begin_arrow_length](/cells/es/python-net/aspose.cells.drawing/line/begin_arrow_length) | Especifica la longitud de la punta de flecha para el comienzo de una línea.|
| [end_arrow_length](/cells/es/python-net/aspose.cells.drawing/line/end_arrow_length) | Especifica la longitud de la punta de flecha para el final de una línea.|
| [begin_arrow_width](/cells/es/python-net/aspose.cells.drawing/line/begin_arrow_width) | Especifica el ancho de la punta de flecha para el comienzo de una línea.|
| [end_arrow_width](/cells/es/python-net/aspose.cells.drawing/line/end_arrow_width) | Especifica el ancho de la punta de flecha para el final de una línea.|
| [theme_color](/cells/es/python-net/aspose.cells.drawing/line/theme_color) | Obtiene y establece el color del tema.|
| [color](/cells/es/python-net/aspose.cells.drawing/line/color) | Representa el Color de la línea.|
| [transparency](/cells/es/python-net/aspose.cells.drawing/line/transparency) | Devuelve o establece el grado de transparencia de la línea como un valor de 0,0 (opaco) a 1,0 (transparente).|
| [style](/cells/es/python-net/aspose.cells.drawing/line/style) | Representa el estilo de la línea.|
| [weight](/cells/es/python-net/aspose.cells.drawing/line/weight) | Obtiene o establece el [WeightType](/cells/es/python-net/aspose.cells.drawing/weighttype) de la línea.|
| [weight_pt](/cells/es/python-net/aspose.cells.drawing/line/weight_pt) | Obtiene o establece el grosor de la línea en unidades de puntos.|
| [weight_px](/cells/es/python-net/aspose.cells.drawing/line/weight_px) | Obtiene o establece el peso de la línea en unidades de píxeles.|
| [formatting_type](/cells/es/python-net/aspose.cells.drawing/line/formatting_type) | Obtiene o establece el tipo de formato.|
| [is_automatic_color](/cells/es/python-net/aspose.cells.drawing/line/is_automatic_color) | Indica si el color de la línea se asigna automáticamente.|
| [is_visible](/cells/es/python-net/aspose.cells.drawing/line/is_visible) | Representa si la línea es visible.|
| [is_auto](/cells/es/python-net/aspose.cells.drawing/line/is_auto) | Indica si este estilo de línea se asigna automáticamente.|
| [gradient_fill](/cells/es/python-net/aspose.cells.drawing/line/gradient_fill) | Representa relleno degradado.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartMarkerType, ChartType
from aspose.cells.drawing import LineType, WeightType
from aspose.pydrawing import Color

workbook = Workbook()
sheet = workbook.worksheets[0]
cells = sheet.cells
cells.get(0, 1).put_value("Income")
cells.get(1, 0).put_value("Company A")
cells.get(2, 0).put_value("Company B")
cells.get(3, 0).put_value("Company C")
cells.get(1, 1).put_value(10000)
cells.get(2, 1).put_value(20000)
cells.get(3, 1).put_value(30000)
chartIndex = sheet.charts.add(ChartType.LINE, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
# Applying a dotted line style on the lines of an NSeries
chart.n_series[0].border.style = LineType.DOT
chart.n_series[0].border.color = Color.red
# Applying a triangular marker style on the data markers of an NSeries
chart.n_series[0].marker.marker_style = ChartMarkerType.TRIANGLE
# Setting the weight of all lines in an NSeries to medium
chart.n_series[0].border.weight = WeightType.MEDIUM_LINE

```

###  Ver también
* módulo [aspose.cells.drawing](..)
* clase [WeightType](/cells/es/python-net/aspose.cells.drawing/weighttype)
