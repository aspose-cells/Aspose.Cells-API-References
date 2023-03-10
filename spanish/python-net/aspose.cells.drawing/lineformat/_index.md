---
title: LineFormat clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 300
url: /es/python-net/aspose.cells.drawing/lineformat/
is_root: false
---
##  LineFormat clase
Representa todos los ajustes de la línea.



**Herencia:** [LineFormat](/cells/python-net/aspose.cells.drawing/lineformat) → 
[FillFormat](/cells/es/python-net/aspose.cells.drawing/fillformat)



El tipo LineFormat expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [type](/cells/es/python-net/aspose.cells.drawing/lineformat/type) |Obtiene y establece el tipo de relleno.|
| [fill_type](/cells/es/python-net/aspose.cells.drawing/lineformat/fill_type) | Obtiene y establece el tipo de relleno|
| [transparency](/cells/es/python-net/aspose.cells.drawing/lineformat/transparency) | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente).|
| [set_type](/cells/es/python-net/aspose.cells.drawing/lineformat/set_type) | Obtiene el tipo de conjunto de formato de relleno.|
| [gradient_fill](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_fill) | Obtiene el objeto [FillFormat.gradient_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#gradient_fill).|
| [texture_fill](/cells/es/python-net/aspose.cells.drawing/lineformat/texture_fill) | Obtiene el objeto [FillFormat.texture_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#texture_fill).|
| [solid_fill](/cells/es/python-net/aspose.cells.drawing/lineformat/solid_fill) | Obtiene el objeto [FillFormat.solid_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#solid_fill).|
| [pattern_fill](/cells/es/python-net/aspose.cells.drawing/lineformat/pattern_fill) | Obtiene el objeto [FillFormat.pattern_fill](/cells/es/python-net/aspose.cells.drawing/fillformat#pattern_fill).|
| [gradient_color_type](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_color_type) | Devuelve el tipo de color de degradado para el relleno especificado.|
| [gradient_style](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_style) | Devuelve el estilo de degradado del relleno especificado.|
| [gradient_color1](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_color1) | Devuelve el color de degradado 1 para el relleno especificado.|
| [gradient_color2](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_color2) | Devuelve el color de degradado 2 para el relleno especificado.|
| [gradient_degree](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_degree) | Devuelve el grado de degradado del relleno especificado.<br/> Solo aplica para Excel 2007.|
| [gradient_variant](/cells/es/python-net/aspose.cells.drawing/lineformat/gradient_variant) | Devuelve la variante de degradado del relleno especificado.<br/> Solo aplica para Excel 2007.|
| [preset_color](/cells/es/python-net/aspose.cells.drawing/lineformat/preset_color) | Devuelve el color predeterminado de degradado para el relleno especificado.|
| [texture](/cells/es/python-net/aspose.cells.drawing/lineformat/texture) | Representa el tipo de textura del relleno especificado.|
| [pattern](/cells/es/python-net/aspose.cells.drawing/lineformat/pattern) | Representa el patrón de visualización de un área.|
| [picture_format_type](/cells/es/python-net/aspose.cells.drawing/lineformat/picture_format_type) | Obtiene y establece el tipo de formato de imagen.|
| [scale](/cells/es/python-net/aspose.cells.drawing/lineformat/scale) | Obtiene y establece la escala de formato de imagen.|
| [image_data](/cells/es/python-net/aspose.cells.drawing/lineformat/image_data) | Obtiene y establece los datos de la imagen de la imagen.|
| [compound_type](/cells/es/python-net/aspose.cells.drawing/lineformat/compound_type) | Especifica el tipo de línea compuesta.|
| [dash_style](/cells/es/python-net/aspose.cells.drawing/lineformat/dash_style) | Especifica el tipo de línea discontinua.|
| [cap_type](/cells/es/python-net/aspose.cells.drawing/lineformat/cap_type) | Especifica las mayúsculas finales.|
| [join_type](/cells/es/python-net/aspose.cells.drawing/lineformat/join_type) | Especifica el tipo de unión de línea.|
| [begin_arrowhead_style](/cells/es/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_style) | Obtiene y establece el tipo de flecha de inicio de la línea.|
| [begin_arrowhead_width](/cells/es/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_width) | Obtiene y establece el tipo de ancho de flecha inicial de la línea.|
| [begin_arrowhead_length](/cells/es/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_length) | Obtiene y establece el tipo de longitud de flecha inicial de la línea.|
| [end_arrowhead_style](/cells/es/python-net/aspose.cells.drawing/lineformat/end_arrowhead_style) | Obtiene y establece el tipo de flecha final de la línea.|
| [end_arrowhead_width](/cells/es/python-net/aspose.cells.drawing/lineformat/end_arrowhead_width) |Obtiene y establece el tipo de ancho de flecha final de la línea.|
| [end_arrowhead_length](/cells/es/python-net/aspose.cells.drawing/lineformat/end_arrowhead_length) | Obtiene y establece el tipo de longitud de flecha final de la línea.|
| [weight](/cells/es/python-net/aspose.cells.drawing/lineformat/weight) | Obtiene o establece el grosor de la línea en unidades de puntos.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/es/python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Establece el relleno especificado en un degradado de dos colores.<br/> Solo aplica para Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/es/python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Establece el relleno especificado en un degradado de dos colores.<br/> Solo aplica para Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/es/python-net/aspose.cells.drawing/lineformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Establece el relleno especificado en un degradado de un color.<br/> Solo aplica para Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/es/python-net/aspose.cells.drawing/lineformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Establece el relleno especificado en un degradado de color predeterminado.<br/> Solo aplica para Excel 2007.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shape = shapes.add_rectangle(1, 0, 1, 0, 50, 100)
lineFmt = shape.line

```

###  Ver también
* módulo [aspose.cells.drawing](..)
* clase [FillFormat](/cells/es/python-net/aspose.cells.drawing/fillformat)
* clase [LineFormat](/cells/es/python-net/aspose.cells.drawing/lineformat)
