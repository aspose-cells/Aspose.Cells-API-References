---
title: FillFormat clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 180
url: /es/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat clase
Encapsula el objeto que representa el formato de relleno de una forma.



El tipo FillFormat expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [type](/cells/es/python-net/aspose.cells.drawing/fillformat/type) |Obtiene y establece el tipo de relleno.|
| [fill_type](/cells/es/python-net/aspose.cells.drawing/fillformat/fill_type) | Obtiene y establece el tipo de relleno|
| [transparency](/cells/es/python-net/aspose.cells.drawing/fillformat/transparency) | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente).|
| [set_type](/cells/es/python-net/aspose.cells.drawing/fillformat/set_type) | Obtiene el tipo de conjunto de formato de relleno.|
| [gradient_fill](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Obtiene el objeto [FillFormat.gradient_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#gradient_fill).|
| [texture_fill](/cells/es/python-net/aspose.cells.drawing/fillformat/texture_fill) | Obtiene el objeto [FillFormat.texture_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#texture_fill).|
| [solid_fill](/cells/es/python-net/aspose.cells.drawing/fillformat/solid_fill) | Obtiene el objeto [FillFormat.solid_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#solid_fill).|
| [pattern_fill](/cells/es/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Obtiene el objeto [FillFormat.pattern_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#pattern_fill).|
| [gradient_color_type](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Devuelve el tipo de color de degradado para el relleno especificado.|
| [gradient_style](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_style) | Devuelve el estilo de degradado del relleno especificado.|
| [gradient_color1](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Devuelve el color de degradado 1 para el relleno especificado.|
| [gradient_color2](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Devuelve el color de degradado 2 para el relleno especificado.|
| [gradient_degree](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Devuelve el grado de degradado del relleno especificado.<br/> Solo aplica para Excel 2007.|
| [gradient_variant](/cells/es/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Devuelve la variante de degradado del relleno especificado.<br/> Solo aplica para Excel 2007.|
| [preset_color](/cells/es/python-net/aspose.cells.drawing/fillformat/preset_color) | Devuelve el color predeterminado de degradado para el relleno especificado.|
| [texture](/cells/es/python-net/aspose.cells.drawing/fillformat/texture) | Representa el tipo de textura del relleno especificado.|
| [pattern](/cells/es/python-net/aspose.cells.drawing/fillformat/pattern) | Representa el patrón de visualización de un área.|
| [picture_format_type](/cells/es/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Obtiene y establece el tipo de formato de imagen.|
| [scale](/cells/es/python-net/aspose.cells.drawing/fillformat/scale) | Obtiene y establece la escala de formato de imagen.|
| [image_data](/cells/es/python-net/aspose.cells.drawing/fillformat/image_data) | Obtiene y establece los datos de la imagen de la imagen.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/es/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Establece el relleno especificado en un degradado de dos colores.<br/> Solo aplica para Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/es/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Establece el relleno especificado en un degradado de dos colores.<br/> Solo aplica para Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/es/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Establece el relleno especificado en un degradado de un color.<br/> Solo aplica para Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/es/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Establece el relleno especificado en un degradado de color predeterminado.<br/> Solo aplica para Excel 2007.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)

```

###  Ver también
* módulo [aspose.cells.drawing](..)
