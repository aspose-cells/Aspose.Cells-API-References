---
title: classe TextBoxCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 690
url: /it/python-net/aspose.cells.drawing/textboxcollection/
is_root: false
---
##  classe TextBoxCollection
Incapsula una raccolta di oggetti [TextBox](/cells/it/python-net/aspose.cells.drawing/textbox).



Il tipo TextBoxCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.drawing/textboxcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [copy_to(array)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add(upper_left_row, upper_left_column, height, width)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/add/#int-int-int-int) | Aggiunge una casella di testo alla raccolta.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.drawing/textboxcollection/binary_search/#TextBox) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get collection object
textBoxCollection = workbook.worksheets[0].text_boxes
# add a textbox
textBoxCollection.add(1, 1, 50, 100)
for tbox in textBoxCollection:
    pass

```

###  Guarda anche
* modulo [aspose.cells.drawing](..)
* classe [TextBox](/cells/it/python-net/aspose.cells.drawing/textbox)
