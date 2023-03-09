---
title: classe SparklineGroupCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 290
url: /it/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  classe SparklineGroupCollection
Incapsula una raccolta di oggetti [SparklineGroup](/cells/it/python-net/aspose.cells.charts/sparklinegroup).



Il tipo SparklineGroupCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [copy_to(array)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add(type, data_range, is_vertical, location_range)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | Aggiunge un elemento [SparklineGroup](/cells/it/python-net/aspose.cells.charts/sparklinegroup) alla raccolta.|
| [clear_sparklines(cell_area)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | Cancella i grafici sparkline che si trovano all'interno di un'area di celle.|
| [clear_sparkline_groups(cell_area)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | Cancella i gruppi di sparkline che si sovrappongono a un'area di celle.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [SparklineGroup](/cells/it/python-net/aspose.cells.charts/sparklinegroup)
