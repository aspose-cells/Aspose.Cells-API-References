---
title: ShapeTextAlignment Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment Klasse
Stellt die Einstellung der Textausrichtung der Form dar;



Der Typ ShapeTextAlignment macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_text_wrapped](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Ruft den Textumbruchtyp der Form ab, die Text enthält, und legt diesen fest.|
| [rotate_text_with_shape](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Gibt an, ob Text mit Form gedreht wird.|
| [text_vertical_overflow](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Ruft den vertikalen Textüberlauftyp des Textfelds ab und legt diesen fest.|
| [text_horizontal_overflow](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Ruft den horizontalen Textüberlauftyp des Textfelds ab und legt diesen fest.|
| [rotation_angle](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Ruft die Rotation der Form ab und legt diese fest.|
| [text_vertical_type](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Ruft die Textrichtung ab und legt sie fest.|
| [auto_size](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |Gibt an, ob die Größe der Form automatisch entsprechend ihrem Inhalt angepasst wird.|
| [text_shape_type](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Ruft den Transformationstyp von Text ab und legt ihn fest.|
| [top_margin_pt](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Gibt den oberen Rand in Punkteinheiten zurück|
| [bottom_margin_pt](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Gibt den unteren Rand in Punkteinheiten zurück|
| [left_margin_pt](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Gibt den linken Rand in Punkteinheiten zurück|
| [right_margin_pt](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Gibt den rechten Rand in Punkteinheiten zurück|
| [is_auto_margin](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Gibt an, ob der Rand des Textrahmens automatisch ist.|
| [number_of_columns](/cells/de/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Ruft die Anzahl der Textspalten im Begrenzungsrechteck ab und legt diese fest.|



###  Beispiel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Siehe auch
* Modul [aspose.cells.drawing.texts](..)
