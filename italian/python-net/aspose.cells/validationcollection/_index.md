---
title: classe ValidationCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1550
url: /it/python-net/aspose.cells/validationcollection/
is_root: false
---
##  classe ValidationCollection
Rappresenta la raccolta di convalida dei dati.



Il tipo ValidationCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/validationcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add()](/cells/it/python-net/aspose.cells/validationcollection/add/#) |Aggiunge una convalida dei dati alla raccolta.|
| [add(ca)](/cells/it/python-net/aspose.cells/validationcollection/add/#CellArea) |Aggiunge una convalida dei dati alla raccolta.|
| [copy_to(array)](/cells/it/python-net/aspose.cells/validationcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [remove_a_cell(row, column)](/cells/it/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Rimuove tutte le impostazioni di convalida sulla cella.|
| [remove_area(ca)](/cells/it/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Rimuove tutte le impostazioni di convalida sull'intervallo..|
| [get_validation_in_cell(row, column)](/cells/it/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Ottiene la convalida applicata alla cella specificata.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Guarda anche
* modulo [aspose.cells](..)
