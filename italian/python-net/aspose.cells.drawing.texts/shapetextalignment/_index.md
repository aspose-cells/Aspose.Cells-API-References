---
title: classe ShapeTextAlignment
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 80
url: /it/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  classe ShapeTextAlignment
Rappresenta l'impostazione dell'allineamento del testo della forma;



Il tipo ShapeTextAlignment espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_text_wrapped](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Ottiene e imposta il tipo di testo a capo della forma che contiene il testo.|
| [rotate_text_with_shape](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Indica se ruotare il testo con la forma.|
| [text_vertical_overflow](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Ottiene e imposta il tipo di overflow verticale del testo della casella di testo.|
| [text_horizontal_overflow](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Ottiene e imposta il tipo di overflow orizzontale del testo della casella di testo.|
| [rotation_angle](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Ottiene e imposta la rotazione della forma.|
| [text_vertical_type](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Ottiene e imposta la direzione del testo.|
| [auto_size](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |Indica se la dimensione della forma viene regolata automaticamente in base al suo contenuto.|
| [text_shape_type](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Ottiene e imposta il tipo di trasformazione del testo.|
| [top_margin_pt](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Restituisce il margine superiore in unità di punti|
| [bottom_margin_pt](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Restituisce il margine inferiore in unità di punti|
| [left_margin_pt](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Restituisce il margine sinistro in unità di punti|
| [right_margin_pt](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Restituisce il margine destro in unità di punti|
| [is_auto_margin](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Indica se il margine della cornice di testo è automatico.|
| [number_of_columns](/cells/it/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Ottiene e imposta il numero di colonne di testo nel rettangolo di delimitazione.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Guarda anche
* modulo [aspose.cells.drawing.texts](..)
