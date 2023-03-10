---
title: classe ChartCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 50
url: /it/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  classe ChartCollection
Incapsula una raccolta di oggetti [Chart](/cells/it/python-net/aspose.cells.charts/chart).



Il tipo ChartCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.charts/chartcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/it/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Aggiunge un grafico alla raccolta.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/it/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Aggiunge un grafico alla raccolta.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/it/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Aggiunge un grafico con modello preimpostato.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/it/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Aggiunge un grafico alla raccolta.|
| [get(index)](/cells/it/python-net/aspose.cells.charts/chartcollection/get/#int) |Aggiungi API for Python tramite .Net.poiché questo[indice int] non è supportato|
| [get(name)](/cells/it/python-net/aspose.cells.charts/chartcollection/get/#str) | Aggiungi API for Python tramite .Net. poiché questo [string Chart] non è supportato|
| [copy_to(array)](/cells/it/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add_floating_chart(type, left, top, width, height)](/cells/it/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Aggiunge un grafico alla raccolta.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [Chart](/cells/it/python-net/aspose.cells.charts/chart)
