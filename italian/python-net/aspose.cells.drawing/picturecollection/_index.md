---
title: classe PictureCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 460
url: /it/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  classe PictureCollection
Incapsula una raccolta di oggetti [Picture](/cells/it/python-net/aspose.cells.drawing/picture).



Il tipo PictureCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.drawing/picturecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Aggiunge un'immagine alla raccolta.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Aggiunge un'immagine alla raccolta.|
| [add(upper_left_row, upper_left_column, stream)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Aggiunge un'immagine alla raccolta.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Aggiunge un'immagine alla raccolta.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Aggiunge un'immagine alla raccolta.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/it/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Aggiunge un'immagine alla raccolta.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempi

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.drawing](..)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
