---
title: CellWatchCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells/cellwatchcollection/
is_root: false
---
##  CellWatchCollection klass
Representerar samlingen av celler på detta kalkylblad som bevakas i "bevakningsfönstret".



Typen CellWatchCollection avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [CellWatchCollection()](/cells/sv/python-net/aspose.cells/cellwatchcollection/__init__/#) | Konstruerar en ny instans av CellWatchCollection|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells/cellwatchcollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(row, column)](/cells/sv/python-net/aspose.cells/cellwatchcollection/add/#int-int) | Lägger till [CellWatch](/cells/sv/python-net/aspose.cells/cellwatch) med rad och kolumn.|
| [add(cell_name)](/cells/sv/python-net/aspose.cells/cellwatchcollection/add/#str) | Lägger till [CellWatch](/cells/sv/python-net/aspose.cells/cellwatch) med namnet på cellen.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells/cellwatchcollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells/cellwatchcollection/binary_search/#CellWatch) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")

```

###  Se även
* modul [aspose.cells](..)
* klass [CellWatch](/cells/sv/python-net/aspose.cells/cellwatch)
