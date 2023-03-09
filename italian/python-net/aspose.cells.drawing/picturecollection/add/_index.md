---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.drawing/picturecollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, stream):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| stream | io.RawIOBase | Oggetto Stream che contiene i dati dell'immagine.|

###  Esempi

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs)

```


##  add(upper_left_row, upper_left_column, file_name) {#int-int-str}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, file_name):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| file_name | str | Nome file immagine.|

###  Esempi

```python

# add a picture
pictures.add(1, 1, "image.jpg")

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
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
    pictures.add(1, 1, 5, 5, fs)

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-str}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| lower_right_row | int | Indice riga in basso a destra|
| lower_right_column | int | Indice colonna in basso a destra|
| file_name | str | Nome file immagine.|

###  Esempi

```python

# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")

```


##  add(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
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
    pictures.add(1, 1, fs, 50, 50)

```


##  add(upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-str-int-int}
Aggiunge un'immagine alla raccolta.


###  ritorna

[Picture](/cells/it/python-net/aspose.cells.drawing/picture) indice oggetto.


```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| file_name | str | Nome file immagine.|
| width_scale | int | Scala della larghezza dell'immagine, una percentuale.|
| height_scale | int | Scala dell'altezza dell'immagine, una percentuale.|

###  Esempi

```python

# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
* classe [PictureCollection](/cells/it/python-net/aspose.cells.drawing/picturecollection)
