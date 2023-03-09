---
title: ShapeTextAlignment clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 80
url: /es/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment clase
Representa la configuración de la alineación del texto de la forma;



El tipo ShapeTextAlignment expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_text_wrapped](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Obtiene y establece el tipo de ajuste de texto de la forma que contiene texto.|
| [rotate_text_with_shape](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Indica si rota el texto con forma.|
| [text_vertical_overflow](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Obtiene y establece el tipo de desbordamiento vertical de texto del cuadro de texto.|
| [text_horizontal_overflow](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Obtiene y establece el tipo de desbordamiento horizontal de texto del cuadro de texto.|
| [rotation_angle](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Obtiene y establece la rotación de la forma.|
| [text_vertical_type](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Obtiene y establece la dirección del texto.|
| [auto_size](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |Indica si el tamaño de la forma se ajusta automáticamente según su contenido.|
| [text_shape_type](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Obtiene y establece el tipo de transformación del texto.|
| [top_margin_pt](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Devuelve el margen superior en unidades de Puntos|
| [bottom_margin_pt](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Devuelve el margen inferior en unidades de Puntos|
| [left_margin_pt](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Devuelve el margen izquierdo en unidades de Puntos|
| [right_margin_pt](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Devuelve el margen derecho en unidades de Puntos|
| [is_auto_margin](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Indica si el margen del cuadro de texto es automático.|
| [number_of_columns](/cells/es/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Obtiene y establece el número de columnas de texto en el rectángulo delimitador.|



###  Ejemplos

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Ver también
* módulo [aspose.cells.drawing.texts](..)
