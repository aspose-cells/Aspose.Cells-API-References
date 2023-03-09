---
title: metodo import_custom_objects
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 640
url: /it/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
Importa oggetti personalizzati.


###  ritorna

Numero totale di righe importate.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| list | list | L'oggetto personalizzato|
| first_row | int | Il numero di riga della prima cella in cui importare.|
| first_column | int | Il numero di colonna della prima cella in cui importare.|
| options | [ImportTableOptions](/cells/it/python-net/aspose.cells/importtableoptions) | Le opzioni di importazione.|
###  Osservazioni

Gli oggetti personalizzati devono essere dello stesso tipo.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

Importa oggetti personalizzati.


###  ritorna

Numero totale di righe importate.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| list | list | L'oggetto personalizzato|
| property_names | list | I nomi delle proprietà.Se è nullo, importeremo tutte le proprietà dell'oggetto.|
| is_property_name_shown | bool | Indica se il nome della proprietà verrà importato nella prima riga.|
| first_row | int | Il numero di riga della prima cella in cui importare.|
| first_column | int | Il numero di colonna della prima cella in cui importare.|
| row_number | int | Numero di righe da importare.|
| insert_rows | bool | Indica se vengono aggiunte ulteriori righe per adattare i dati.|
| date_format_string | str | Stringa del formato della data per le celle.|
| convert_string_to_number | bool | Indica se questo metodo proverà a convertire la stringa in numero.|
###  Osservazioni

Gli oggetti personalizzati devono essere dello stesso tipo.


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
