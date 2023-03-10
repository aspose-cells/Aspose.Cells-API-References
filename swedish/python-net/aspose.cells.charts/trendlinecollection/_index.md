---
title: TrendlineCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 340
url: /sv/python-net/aspose.cells.charts/trendlinecollection/
is_root: false
---
##  TrendlineCollection klass
Representerar en samling av alla [Trendline](/cells/sv/python-net/aspose.cells.charts/trendline)-objekt för den angivna dataserien.



Typen TrendlineCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(type)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType) | Lägger till ett [Trendline](/cells/sv/python-net/aspose.cells.charts/trendline)-objekt till den här samlingen med angiven typ.|
| [add(type, name)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType-str) | Lägger till ett [Trendline](/cells/sv/python-net/aspose.cells.charts/trendline)-objekt till den här samlingen med angiven typ och namn.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.charts/trendlinecollection/binary_search/#Trendline) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
worksheet.cells.get("A1").put_value(50)
worksheet.cells.get("A2").put_value(100)
worksheet.cells.get("A3").put_value(150)
worksheet.cells.get("A4").put_value(200)
worksheet.cells.get("B1").put_value(60)
worksheet.cells.get("B2").put_value(32)
worksheet.cells.get("B3").put_value(50)
worksheet.cells.get("B4").put_value(40)
# Adding a chart to the worksheet
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 3, 3, 15, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:a3", True)
chart.n_series[0].trend_lines.add(TrendlineType.LINEAR, "MyTrendLine")
line = chart.n_series[0].trend_lines[0]
line.display_equation = True
line.display_r_squared = True
line.color = Color.red

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [Trendline](/cells/sv/python-net/aspose.cells.charts/trendline)
