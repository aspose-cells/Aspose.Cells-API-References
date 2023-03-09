---
title: classe PivotTableCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 110
url: /it/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  classe PivotTableCollection
Rappresenta la raccolta di tutti gli oggetti tabella pivot nel foglio di lavoro specificato.



Il tipo PivotTableCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.|
| [add(source_data, row, column, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.|
| [add(pivot_table, row, column, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [remove_at(index, keep_data)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | Elimina la tabella pivot in corrispondenza dell'indice specificato|
| [binary_search(item)](/cells/it/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempi

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.pivot](..)
