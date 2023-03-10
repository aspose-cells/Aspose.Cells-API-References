---
title: classe RowCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1310
url: /it/python-net/aspose.cells/rowcollection/
is_root: false
---
##  classe RowCollection
Raccoglie gli oggetti [Row](/cells/it/python-net/aspose.cells/row) che rappresentano le singole righe in un foglio di lavoro.



Il tipo RowCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [count](/cells/it/python-net/aspose.cells/rowcollection/count) | Ottiene il numero di righe in questa raccolta.|



Ottiene un oggetto [Row](/cells/it/python-net/aspose.cells/row) in base all'indice di riga specificato. L'oggetto Row dell'indice di riga specificato verrà istanziato se non esiste prima.
###  Indicizzatore
| Nome| Descrizione|
| :- | :- |
| [index] |  |


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get_row_by_index(index)](/cells/it/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Ottiene l'oggetto riga in base alla posizione nell'elenco.|
| [clear()](/cells/it/python-net/aspose.cells/rowcollection/clear/#) | Cancella tutte le righe e le celle.|
| [remove_at(index)](/cells/it/python-net/aspose.cells/rowcollection/remove_at/#int) | Rimuove la riga in corrispondenza dell'indice specificato|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Row](/cells/it/python-net/aspose.cells/row)
