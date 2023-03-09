---
title: classe CommentCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 290
url: /it/python-net/aspose.cells/commentcollection/
is_root: false
---
##  classe CommentCollection
Incapsula una raccolta di oggetti [Comment](/cells/it/python-net/aspose.cells/comment).



Il tipo CommentCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/commentcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/it/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Aggiunge un commento in thread.|
| [add_threaded_comment(cell_name, text, author)](/cells/it/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Aggiunge un commento in thread.|
| [get_threaded_comments(row, column)](/cells/it/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Ottiene i commenti in thread per indice di riga e colonna.|
| [get_threaded_comments(cell_name)](/cells/it/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Ottiene i commenti in thread in base al nome della cella.|
| [add(row, column)](/cells/it/python-net/aspose.cells/commentcollection/add/#int-int) | Aggiunge un commento alla raccolta.|
| [add(cell_name)](/cells/it/python-net/aspose.cells/commentcollection/add/#str) | Aggiunge un commento alla raccolta.|
| [remove_at(cell_name)](/cells/it/python-net/aspose.cells/commentcollection/remove_at/#str) | Rimuove il commento della cella specifica.|
| [remove_at(row, column)](/cells/it/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Rimuove il commento della cella specifica.|
| [copy_to(array)](/cells/it/python-net/aspose.cells/commentcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Comment](/cells/it/python-net/aspose.cells/comment)
