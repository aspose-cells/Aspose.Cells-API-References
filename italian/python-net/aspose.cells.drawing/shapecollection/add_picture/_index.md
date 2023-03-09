---
title: metodo add_picture
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 210
url: /it/python-net/aspose.cells.drawing/shapecollection/add_picture/
is_root: false
---
##  add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) Oggetto immagine.


```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| lower_right_row | int | Indice riga in basso a destra|
| lower_right_column | int | Indice colonna in basso a destra|
| stream | io.RawIOBase | Oggetto Stream che contiene i dati dell'immagine.|

###  Esempi

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 0, 1, 0, fs)

```


##  add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) Oggetto immagine.


```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| stream | io.RawIOBase | Oggetto Stream che contiene i dati dell'immagine.|
| width_scale | int | Scala della larghezza dell'immagine, una percentuale.|
| height_scale | int | Scala dell'altezza dell'immagine, una percentuale.|

###  Esempi

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 1, fs, 50, 60)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
