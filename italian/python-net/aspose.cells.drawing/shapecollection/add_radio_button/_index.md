---
title: metodo add_radio_button
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 230
url: /it/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un RadioButton al foglio di lavoro.


###  ritorna

Un oggetto RadioButton.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di RadioButton dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di RadioButton dalla relativa colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di RadioButton, in unità di pixel.|
| width | int | Rappresenta la larghezza di RadioButton, in unità di pixel.|

###  Esempi

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
