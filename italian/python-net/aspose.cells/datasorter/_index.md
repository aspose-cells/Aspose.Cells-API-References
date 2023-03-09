---
title: classe DataSorter
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 420
url: /it/python-net/aspose.cells/datasorter/
is_root: false
---
##  classe DataSorter
Descrizione sintetica per DataSorter.



Il tipo DataSorter espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [keys](/cells/it/python-net/aspose.cells/datasorter/keys) | Ottiene l'elenco delle chiavi dell'ordinatore dati.|
| [has_headers](/cells/it/python-net/aspose.cells/datasorter/has_headers) | Indica se l'intervallo ha intestazioni.|
| [key1](/cells/it/python-net/aspose.cells/datasorter/key1) |Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).|
| [order1](/cells/it/python-net/aspose.cells/datasorter/order1) | Rappresenta l'ordinamento della prima chiave.|
| [key2](/cells/it/python-net/aspose.cells/datasorter/key2) | Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).|
| [order2](/cells/it/python-net/aspose.cells/datasorter/order2) | Rappresenta l'ordinamento della seconda chiave.|
| [key3](/cells/it/python-net/aspose.cells/datasorter/key3) | Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).|
| [order3](/cells/it/python-net/aspose.cells/datasorter/order3) | Rappresenta l'ordinamento della terza chiave.|
| [sort_left_to_right](/cells/it/python-net/aspose.cells/datasorter/sort_left_to_right) | Vero significa che l'orientamento dell'ordinamento è da sinistra a destra.<br/>Falso significa che l'orientamento dell'ordinamento è dall'alto verso il basso.<br/> Il valore predefinito è falso.|
| [case_sensitive](/cells/it/python-net/aspose.cells/datasorter/case_sensitive) | Ottiene e imposta la distinzione tra maiuscole e minuscole durante il confronto di stringhe.|
| [sort_as_number](/cells/it/python-net/aspose.cells/datasorter/sort_as_number) | Indica se ordinare qualcosa che assomiglia a un numero.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_key(key, order)](/cells/it/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Aggiunge l'indice di colonna ordinato e l'ordinamento.|
| [add_key(key, order, custom_list)](/cells/it/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Aggiunge l'indice di colonna ordinato e l'ordinamento con l'elenco di ordinamento personalizzato.|
| [add_key(key, type, order, custom_list)](/cells/it/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Aggiunge l'indice di colonna ordinato e l'ordinamento con l'elenco di ordinamento personalizzato.|
| [add_key(key, order, custom_list)](/cells/it/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Aggiunge l'indice di colonna ordinato e l'ordinamento con l'elenco di ordinamento personalizzato.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Ordina i dati dell'area.|
| [sort(cells, area)](/cells/it/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Ordina i dati della zona.|
| [sort()](/cells/it/python-net/aspose.cells/datasorter/sort/#) | Ordina i dati nell'intervallo.|
| [clear()](/cells/it/python-net/aspose.cells/datasorter/clear/#) | Cancella tutte le impostazioni.|



###  Esempio

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
