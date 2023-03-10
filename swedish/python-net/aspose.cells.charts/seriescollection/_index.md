---
title: SeriesCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 240
url: /sv/python-net/aspose.cells.charts/seriescollection/
is_root: false
---
##  SeriesCollection klass
Kapslar in en samling av [Series](/cells/sv/python-net/aspose.cells.charts/series) objekt.



Typen SeriesCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [category_data](/cells/sv/python-net/aspose.cells.charts/seriescollection/category_data) | Hämtar eller ställer in intervallet för kategoriaxelvärden.<br/> Det kan vara ett cellintervall (som "d1:e10"),<br/> eller en sekvens av värden (som,"{2,6,8,10}").|
| [second_category_data](/cells/sv/python-net/aspose.cells.charts/seriescollection/second_category_data) | Hämtar eller ställer in intervallet för andra kategorins axelvärden.<br/> Det kan vara ett cellintervall (som "d1:e10"),<br/> eller en sekvens av värden (som,"{2,6,8,10}").<br/> Effekter endast när vissa ASeries plottar på den andra axeln.|
| [is_color_varied](/cells/sv/python-net/aspose.cells.charts/seriescollection/is_color_varied) | Representerar om färgen på punkterna varieras.|
| [capacity](/cells/sv/python-net/aspose.cells.charts/seriescollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(area, is_vertical)](/cells/sv/python-net/aspose.cells.charts/seriescollection/add/#str-bool) | Lägger till samlingen [SeriesCollection](/cells/sv/python-net/aspose.cells.charts/seriescollection) i ett diagram.|
| [add(area, is_vertical, check_labels)](/cells/sv/python-net/aspose.cells.charts/seriescollection/add/#str-bool-bool) | Lägger till samlingen [SeriesCollection](/cells/sv/python-net/aspose.cells.charts/seriescollection) i ett diagram.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.charts/seriescollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.charts/seriescollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [get_series_by_order(order)](/cells/sv/python-net/aspose.cells.charts/seriescollection/get_series_by_order/#int) | Hämtar elementet [Series](/cells/sv/python-net/aspose.cells.charts/series) efter beställning.|
| [change_series_order(source_index, dest_index)](/cells/sv/python-net/aspose.cells.charts/seriescollection/change_series_order/#int-int) | Ändrar direkt beställningarna för de två serierna.|
| [set_series_names(start_index, area, is_vertical)](/cells/sv/python-net/aspose.cells.charts/seriescollection/set_series_names/#int-str-bool) | Ställer in namnet på alla serier i diagrammet.|
| [add_r1c1(area, is_vertical)](/cells/sv/python-net/aspose.cells.charts/seriescollection/add_r1c1/#str-bool) | Lägger till samlingen [SeriesCollection](/cells/sv/python-net/aspose.cells.charts/seriescollection) i ett diagram.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.charts/seriescollection/binary_search/#Series) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [Series](/cells/sv/python-net/aspose.cells.charts/series)
* klass [SeriesCollection](/cells/sv/python-net/aspose.cells.charts/seriescollection)
