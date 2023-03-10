---
title: ShapeTextAlignment klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 80
url: /sv/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment klass
Representerar inställningen av formens textjustering;



Typen ShapeTextAlignment avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_text_wrapped](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Hämtar och ställer in texttypen för formen som innehåller text.|
| [rotate_text_with_shape](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Anger om text roteras med form.|
| [text_vertical_overflow](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Hämtar och ställer in textrutans vertikala överflödestyp.|
| [text_horizontal_overflow](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Hämtar och ställer in textrutans horisontella överflödestyp.|
| [rotation_angle](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Får och ställer in formens rotation.|
| [text_vertical_type](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Hämtar och anger textriktningen.|
| [auto_size](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |Indikerar om storleken på formen justeras automatiskt efter dess innehåll.|
| [text_shape_type](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Hämtar och ställer in transformeringstypen för text.|
| [top_margin_pt](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Returnerar den övre marginalen i poängenhet|
| [bottom_margin_pt](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Returnerar bottenmarginalen i poängenhet|
| [left_margin_pt](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Returnerar den vänstra marginalen i poängenhet|
| [right_margin_pt](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Returnerar högermarginalen i poängenhet|
| [is_auto_margin](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Anger om marginalen på textramen är automatisk.|
| [number_of_columns](/cells/sv/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Hämtar och ställer in antalet kolumner med text i den avgränsande rektangeln.|



###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Se även
* modul [aspose.cells.drawing.texts](..)
