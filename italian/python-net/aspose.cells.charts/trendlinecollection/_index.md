---
title: classe TrendlineCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 340
url: /it/python-net/aspose.cells.charts/trendlinecollection/
is_root: false
---
##  classe TrendlineCollection
Rappresenta una raccolta di tutti gli oggetti [Trendline](/cells/it/python-net/aspose.cells.charts/trendline) per la serie di dati specificata.



Il tipo TrendlineCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.charts/trendlinecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(type)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType) | Aggiunge un oggetto [Trendline](/cells/it/python-net/aspose.cells.charts/trendline) a questa raccolta con il tipo specificato.|
| [add(type, name)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType-str) | Aggiunge un oggetto [Trendline](/cells/it/python-net/aspose.cells.charts/trendline) a questa raccolta con il tipo e il nome specificati.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.charts/trendlinecollection/binary_search/#Trendline) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [Trendline](/cells/it/python-net/aspose.cells.charts/trendline)
