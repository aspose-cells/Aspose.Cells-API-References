---
title: classe HorizontalPageBreakCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 760
url: /it/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  classe HorizontalPageBreakCollection
Incapsula una raccolta di oggetti [HorizontalPageBreak](/cells/it/python-net/aspose.cells/horizontalpagebreak).



Il tipo HorizontalPageBreakCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(row, start_column, end_column)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta.|
| [add(row)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta.|
| [add(row, column)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta.|
| [add(cell_name)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Aggiunge un'interruzione di pagina orizzontale alla raccolta.|
| [copy_to(array)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [HorizontalPageBreak](/cells/it/python-net/aspose.cells/horizontalpagebreak)
