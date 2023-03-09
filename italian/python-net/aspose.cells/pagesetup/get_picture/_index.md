---
title: metodo get_picture
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 120
url: /it/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Ottiene l'oggetto [Picture](/cells/it/python-net/aspose.cells.drawing/picture) dell'intestazione/piè di pagina.


###  ritorna

Restituisce l'oggetto [Picture](/cells/it/python-net/aspose.cells.drawing/picture).
Restituisce null se non è presente alcuna immagine.


```python
def get_picture(self, is_header, section):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| is_header | bool | Indica se si trova nell'intestazione o nel piè di pagina.|
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Ottiene l'oggetto [Picture](/cells/it/python-net/aspose.cells.drawing/picture) dell'intestazione/piè di pagina.


###  ritorna

Restituisce l'oggetto [Picture](/cells/it/python-net/aspose.cells.drawing/picture).


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| is_first | bool | Indica se ottenere l'immagine dell'intestazione/piè di pagina della prima pagina.|
| is_even | bool | Indica se ottenere l'immagine dell'intestazione/piè di pagina pari.|
| is_header | bool | Indica se ottenere l'immagine dell'intestazione/piè di pagina.|
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PageSetup](/cells/it/python-net/aspose.cells/pagesetup)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
