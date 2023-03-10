---
title: metodo add_active_x_control
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Crea un controllo Activex.


###  ritorna




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | Il tipo di controllo.|
| top_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di Shape dalla riga sinistra, in unità di pixel.|
| left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di Shape dalla colonna di sinistra, in unità di pixel.|
| width | int | Rappresenta la larghezza di Shape, in unità di pixel.|
| height | int | Rappresenta l'altezza di Shape, in unità di pixel.|

###  Esempio

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
