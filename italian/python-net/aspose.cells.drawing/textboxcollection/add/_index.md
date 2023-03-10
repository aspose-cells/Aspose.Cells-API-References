---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.drawing/textboxcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width) {#int-int-int-int}
Aggiunge una casella di testo alla raccolta.


###  ritorna

[TextBox](/cells/it/python-net/aspose.cells.drawing/textbox) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| height | int | Altezza della casella di testo, in unità di pixel.|
| width | int | Larghezza della casella di testo, in unità di pixel.|

###  Esempio

```python

# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [TextBox](/cells/it/python-net/aspose.cells.drawing/textbox)
* classe [TextBoxCollection](/cells/it/python-net/aspose.cells.drawing/textboxcollection)
