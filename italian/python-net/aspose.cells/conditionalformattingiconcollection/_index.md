---
title: classe ConditionalFormattingIconCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 320
url: /it/python-net/aspose.cells/conditionalformattingiconcollection/
is_root: false
---
##  classe ConditionalFormattingIconCollection
Rappresenta una raccolta di [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon) oggetti.



Il tipo ConditionalFormattingIconCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(type, index)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/add/#IconSetType-int) | Aggiunge l'oggetto [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon).|
| [add(cficon)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/add/#ConditionalFormattingIcon) | Aggiunge l'oggetto [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon).|
| [copy_to(array)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/index_of/#ConditionalFormattingIcon-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/index_of/#ConditionalFormattingIcon-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/conditionalformattingiconcollection/binary_search/#ConditionalFormattingIcon) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Get Conditional Formatting
cformattings = sheet.conditional_formattings
# Adds an empty conditional formatting
index = cformattings.add()
# Get newly added Conditional formatting
fcs = cformattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Sets condition
idx = fcs.add_condition(FormatConditionType.ICON_SET)
cond = fcs[idx]
# Sets condition's type
cond.icon_set.type = IconSetType.ARROWS_GRAY3
# Add custom iconset condition.
cfIcon = cond.icon_set.cf_icons[0]
cfIcon.type = IconSetType.ARROWS3
cfIcon.index = 0
cfIcon1 = cond.icon_set.cf_icons[1]
cfIcon1.type = IconSetType.ARROWS_GRAY3
cfIcon1.index = 1
cfIcon2 = cond.icon_set.cf_icons[2]
cfIcon2.type = IconSetType.BOXES5
cfIcon2.index = 2
# Saving the Excel file
workbook.save("output.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [ConditionalFormattingIcon](/cells/it/python-net/aspose.cells/conditionalformattingicon)
