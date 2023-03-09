---
title: metodo set_embedded_object
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 170
url: /it/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Imposta i dati oggetto incorporati.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| link_to_file | bool | Indica se l'oggetto si collega al file.Se vero, il parametro objectData viene ignorato.|
| object_data | bytes | I dati dell'oggetto incorporato.|
| source_file_name | str | Il nome del file.|
| display_as_icon | bool | Indica se visualizzare l'oggetto come icona.<br/> Se vero, i dati dell'immagine originale saranno coperti dall'icona.|
| label | str | L'etichetta dell'icona Funziona solo quando displayAsIcon è true.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Imposta i dati oggetto incorporati.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| link_to_file | bool | Indica se l'oggetto si collega al file.Se vero, il parametro objectData viene ignorato.|
| object_data | bytes | I dati dell'oggetto incorporato.|
| source_file_name | str | Il nome del file.|
| display_as_icon | bool | Indica se visualizzare l'oggetto come icona.<br/> Se vero, i dati dell'immagine originale saranno coperti dall'icona.|
| label | str | L'etichetta dell'icona Funziona solo quando displayAsIcon è true.|
| update_icon | bool | Indica se aggiornare automaticamente l'icona.|
###  Osservazioni

Poiché Aspose può aggiornare incorporare tutte le icone dei file, quindi è meglio che tu possa aggiungere l'icona corretta con `update_icon` come false.


###  Guarda anche

* modulo [aspose.cells.drawing](../../)
* classe [OleObject](/cells/it/python-net/aspose.cells.drawing/oleobject)
