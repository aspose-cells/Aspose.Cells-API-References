---
title: add_word_art método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 350
url: /es/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Agrega WordArt predeterminado desde Excel 2007.s


###  Devoluciones




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/es/python-net/aspose.cells.drawing/presetwordartstyle) |El estilo de WordArt preestablecido.|
| text | str | El texto.|
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int |Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de la forma, en unidades de píxel.|
| width | int | Representa el ancho de la forma, en unidades de píxel.|

###  Ejemplo

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
