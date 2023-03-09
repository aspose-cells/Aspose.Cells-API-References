---
title: ChartDataTable klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable klass
Representerar en diagramdatatabell.



Typen ChartDataTable avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [font](/cells/sv/python-net/aspose.cells.charts/chartdatatable/font) | Hämtar ett [ChartDataTable.font](/cells/sv/python-net/aspose.cells.charts/chartdatatable#font)-objekt som representerar teckensnittsinställningen för den angivna diagramdatatabellen.|
| [auto_scale_font](/cells/sv/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | Sant om texten i objektet ändrar teckenstorlek när objektstorleken ändras.<br/> Standardvärdet är True.|
| [background_mode](/cells/sv/python-net/aspose.cells.charts/chartdatatable/background_mode) | Hämtar och ställer in visningsläget för bakgrunden|
| [background](/cells/sv/python-net/aspose.cells.charts/chartdatatable/background) | Hämtar och ställer in visningsläget för bakgrunden|
| [has_border_horizontal](/cells/sv/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |Sant om diagramdatatabellen har horisontella cellkanter|
| [has_border_vertical](/cells/sv/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | Sant om diagramdatatabellen har vertikala cellkanter|
| [has_border_outline](/cells/sv/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | Sant om diagramdatatabellen har konturgränser|
| [show_legend_key](/cells/sv/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | Sant om nyckeln för dataetikettförklaringen är synlig.|
| [border](/cells/sv/python-net/aspose.cells.charts/chartdatatable/border) | Returnerar ett Border-objekt som representerar objektets kant|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells.charts](..)
