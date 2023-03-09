---
title: metodo add_auto_shape
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Aggiunge una forma al foglio di lavoro.


###  ritorna

Un oggetto Forma.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [AutoShapeType](/cells/it/python-net/aspose.cells.drawing/autoshapetype) | Tipo di forma automatica.|
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di Shape dalla riga sinistra, in unità di pixel.|
| upper_left_column | int |Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di Shape dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di Shape, in unità di pixel.|
| width | int | Rappresenta la larghezza di Shape, in unità di pixel.|
###  Osservazioni

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox
###  Esempio


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
