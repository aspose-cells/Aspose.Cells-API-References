---
title: ErrorBar clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 150
url: /es/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  ErrorBar clase
Representa la barra de error de la serie de datos.



**Herencia:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/es/python-net/aspose.cells.drawing/line)



El tipo ErrorBar expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [compound_type](/cells/es/python-net/aspose.cells.charts/errorbar/compound_type) | Especifica el tipo de línea compuesta|
| [dash_type](/cells/es/python-net/aspose.cells.charts/errorbar/dash_type) | Especifica el tipo de línea discontinua|
| [cap_type](/cells/es/python-net/aspose.cells.charts/errorbar/cap_type) | Especifica las mayúsculas finales.|
| [join_type](/cells/es/python-net/aspose.cells.charts/errorbar/join_type) | Especifica las tapas de unión.|
| [begin_type](/cells/es/python-net/aspose.cells.charts/errorbar/begin_type) |Especifica una punta de flecha para el comienzo de una línea.|
| [end_type](/cells/es/python-net/aspose.cells.charts/errorbar/end_type) | Especifica una punta de flecha para el final de una línea.|
| [begin_arrow_length](/cells/es/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Especifica la longitud de la punta de flecha para el comienzo de una línea.|
| [end_arrow_length](/cells/es/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Especifica la longitud de la punta de flecha para el final de una línea.|
| [begin_arrow_width](/cells/es/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Especifica el ancho de la punta de flecha para el comienzo de una línea.|
| [end_arrow_width](/cells/es/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Especifica el ancho de la punta de flecha para el final de una línea.|
| [theme_color](/cells/es/python-net/aspose.cells.charts/errorbar/theme_color) | Obtiene y establece el color del tema.|
| [color](/cells/es/python-net/aspose.cells.charts/errorbar/color) | Representa el Color de la línea.|
| [transparency](/cells/es/python-net/aspose.cells.charts/errorbar/transparency) | Devuelve o establece el grado de transparencia de la línea como un valor de 0,0 (opaco) a 1,0 (transparente).|
| [style](/cells/es/python-net/aspose.cells.charts/errorbar/style) | Representa el estilo de la línea.|
| [weight](/cells/es/python-net/aspose.cells.charts/errorbar/weight) | Obtiene o establece el [WeightType](/cells/es/python-net/aspose.cells.drawing/weighttype) de la línea.|
| [weight_pt](/cells/es/python-net/aspose.cells.charts/errorbar/weight_pt) | Obtiene o establece el grosor de la línea en unidades de puntos.|
| [weight_px](/cells/es/python-net/aspose.cells.charts/errorbar/weight_px) | Obtiene o establece el peso de la línea en unidades de píxeles.|
| [formatting_type](/cells/es/python-net/aspose.cells.charts/errorbar/formatting_type) | Obtiene o establece el tipo de formato.|
| [is_automatic_color](/cells/es/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Indica si el color de la línea se asigna automáticamente.|
| [is_visible](/cells/es/python-net/aspose.cells.charts/errorbar/is_visible) | Representa si la línea es visible.|
| [is_auto](/cells/es/python-net/aspose.cells.charts/errorbar/is_auto) | Indica si este estilo de línea se asigna automáticamente.|
| [gradient_fill](/cells/es/python-net/aspose.cells.charts/errorbar/gradient_fill) | Representa relleno degradado.|
| [type](/cells/es/python-net/aspose.cells.charts/errorbar/type) |Representa el tipo de cantidad de la barra de error.|
| [display_type](/cells/es/python-net/aspose.cells.charts/errorbar/display_type) | Representa el tipo de visualización de la barra de error.|
| [amount](/cells/es/python-net/aspose.cells.charts/errorbar/amount) | Representa la cantidad de barra de error.<br/> La cantidad debe ser mayor o igual a cero.|
| [show_marker_t_top](/cells/es/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Indica si hay barras de error de formato con una T-top.|
| [plus_value](/cells/es/python-net/aspose.cells.charts/errorbar/plus_value) | Representa una cantidad de error positiva cuando el tipo de barra de error es Personalizado.|
| [minus_value](/cells/es/python-net/aspose.cells.charts/errorbar/minus_value) | Representa la cantidad de error negativa cuando el tipo de barra de error es Personalizado.|



###  Ejemplos

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.NSeries)):
    aseries = chart.n_series[i]
    aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
    aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
    aseries.y_error_bar.amount = 5

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [ErrorBar](/cells/es/python-net/aspose.cells.charts/errorbar)
* clase [Line](/cells/es/python-net/aspose.cells.drawing/line)
* clase [WeightType](/cells/es/python-net/aspose.cells.drawing/weighttype)
