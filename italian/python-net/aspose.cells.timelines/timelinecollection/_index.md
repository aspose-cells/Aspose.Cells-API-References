---
title: classe TimelineCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.timelines/timelinecollection/
is_root: false
---
##  classe TimelineCollection
Specifica la raccolta di tutti gli oggetti della sequenza temporale nel foglio di lavoro specificato.
A causa di MS Excel, Excel 2003 non supporta la linea temporale.



Il tipo TimelineCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.timelines/timelinecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(pivot, row, column, base_field_name)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [add(pivot, dest_cell_name, base_field_name)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-str) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [add(pivot, row, column, base_field_index)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [add(pivot, dest_cell_name, base_field_index)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-int) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [add(pivot, row, column, base_field)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [add(pivot, dest_cell_name, base_field)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati|
| [copy_to(array)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.timelines/timelinecollection/binary_search/#Timeline) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.timelines](..)
