---
title: classe VbaModuleCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
##  classe VbaModuleCollection
Rappresenta la lista di [VbaModule](/cells/it/python-net/aspose.cells.vba/vbamodule)



Il tipo VbaModuleCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(sheet)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) |Aggiunge moduli per un foglio di lavoro.|
| [add(type, name)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) | Aggiunge modulo.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add_designer_storage(name, data)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) | Rappresenta i dati di Designer.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempi

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Guarda anche
* modulo [aspose.cells.vba](..)
* classe [VbaModule](/cells/it/python-net/aspose.cells.vba/vbamodule)
