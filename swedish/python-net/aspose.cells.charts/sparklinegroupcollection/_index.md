---
title: SparklineGroupCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 290
url: /sv/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection klass
Kapslar in en samling av [SparklineGroup](/cells/sv/python-net/aspose.cells.charts/sparklinegroup) objekt.



Typen SparklineGroupCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [copy_to(array)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [add(type, data_range, is_vertical, location_range)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | Lägger till ett [SparklineGroup](/cells/sv/python-net/aspose.cells.charts/sparklinegroup) föremål till samlingen.|
| [clear_sparklines(cell_area)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | Rensar gnistlinjerna som finns inuti ett område av celler.|
| [clear_sparkline_groups(cell_area)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | Rensar sparklinegrupperna som överlappar ett område med celler.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

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

###  Se även
* modul [aspose.cells.charts](..)
* klass [SparklineGroup](/cells/sv/python-net/aspose.cells.charts/sparklinegroup)
