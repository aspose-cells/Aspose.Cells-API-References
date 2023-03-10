---
title: metodo register_add_in_function
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 170
url: /it/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Aggiunge la funzione addin nella cartella di lavoro


###  ritorna

URL del file addin che contiene le funzioni addin


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| id | int | ID dei dati che contengono funzioni aggiuntive,<br/> può essere ottenuto dalla prima chiamata di [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/it/python-net/aspose.cells/worksheetcollection/register_add_in_function) per lo stesso file addin.|
| function_name | str | il nome della funzione addin|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Aggiunge la funzione addin nella cartella di lavoro


###  ritorna

ID dei dati che contengono una determinata funzione aggiuntiva


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| add_in_file | str | il file contiene le funzioni addin|
| function_name | str | il nome della funzione addin|
| lib | bool | se il file aggiuntivo specificato si trova nella directory o nella sottodirectory della libreria del componente aggiuntivo della cartella di lavoro.<br/>Questo flag ha effetto e fa la differenza quando dato addInFile è di percorso relativo:<br/> true indica che il percorso è relativo alla libreria del componente aggiuntivo e false indica che il percorso è relativo a questa cartella di lavoro.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [WorksheetCollection](/cells/it/python-net/aspose.cells/worksheetcollection)
