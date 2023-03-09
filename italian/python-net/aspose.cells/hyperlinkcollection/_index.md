---
title: classe HyperlinkCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 800
url: /it/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  classe HyperlinkCollection
Incapsula una raccolta di oggetti [Hyperlink](/cells/it/python-net/aspose.cells/hyperlink).



Il tipo HyperlinkCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/hyperlinkcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/it/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.|
| [add(cell_name, total_rows, total_columns, address)](/cells/it/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/it/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.|
| [copy_to(array)](/cells/it/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Hyperlink](/cells/it/python-net/aspose.cells/hyperlink)
