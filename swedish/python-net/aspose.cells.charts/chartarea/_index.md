---
title: ChartArea klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea klass
Kapslar in objektet som representerar diagramområdet i kalkylbladet.



**Arv:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/sv/python-net/aspose.cells.charts/chartframe)



Typen ChartArea avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_inner_mode](/cells/sv/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Anger om storleken på plottytans storlek inkluderar bockmarkeringarna och axeletiketterna.<br/> False anger att storleken ska avgöra storleken på tomtområdet, bockarna och axeletiketterna.|
| [border](/cells/sv/python-net/aspose.cells.charts/chartarea/border) | Får [Line](/cells/sv/python-net/aspose.cells.drawing/line).|
| [area](/cells/sv/python-net/aspose.cells.charts/chartarea/area) | Får [ChartFrame.area](/cells/sv/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/sv/python-net/aspose.cells.charts/chartarea/text_font) | Hämtar ett [ChartFrame.font](/cells/sv/python-net/aspose.cells.charts/chartframe#font)-objekt av det angivna ChartFrame-objektet.|
| [text_options](/cells/sv/python-net/aspose.cells.charts/chartarea/text_options) | Hämtar och ställer in alternativen för texten.|
| [font](/cells/sv/python-net/aspose.cells.charts/chartarea/font) | Hämtar ett [ChartArea.font](/cells/sv/python-net/aspose.cells.charts/chartarea#font)-objekt av det angivna chartarea-objektet.|
| [auto_scale_font](/cells/sv/python-net/aspose.cells.charts/chartarea/auto_scale_font) | Sant om texten i objektet ändrar teckenstorlek när objektstorleken ändras. Standardvärdet är True.|
| [background_mode](/cells/sv/python-net/aspose.cells.charts/chartarea/background_mode) | Hämtar och ställer in visningsläget för bakgrunden|
| [background](/cells/sv/python-net/aspose.cells.charts/chartarea/background) | Hämtar och ställer in visningsläget för bakgrunden|
| [is_automatic_size](/cells/sv/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Indikerar om kartramen har automatisk storlek.|
| [x](/cells/sv/python-net/aspose.cells.charts/chartarea/x) | Hämtar eller hämtar den horisontella förskjutningen från kolumnen i det övre vänstra hörnet.|
| [y](/cells/sv/python-net/aspose.cells.charts/chartarea/y) | Hämtar eller hämtar den vertikala förskjutningen från dess övre vänstra hörnrad.|
| [height](/cells/sv/python-net/aspose.cells.charts/chartarea/height) | Hämtar eller ställer in den vertikala förskjutningen från dess nedre högra hörnrad.|
| [width](/cells/sv/python-net/aspose.cells.charts/chartarea/width) | Hämtar eller ställer in den horisontella förskjutningen från kolumnen i det nedre högra hörnet.|
| [shadow](/cells/sv/python-net/aspose.cells.charts/chartarea/shadow) | Sant om ramen har en skugga.|
| [shape_properties](/cells/sv/python-net/aspose.cells.charts/chartarea/shape_properties) | Hämtar objektet [ChartFrame.shape_properties](/cells/sv/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/sv/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Anger om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är inställda.|
| [default_x](/cells/sv/python-net/aspose.cells.charts/chartarea/default_x) | Representerar x av standardposition|
| [default_y](/cells/sv/python-net/aspose.cells.charts/chartarea/default_y) | Representerar y för standardposition|
| [default_width](/cells/sv/python-net/aspose.cells.charts/chartarea/default_width) | Representerar bredden på standardpositionen|
| [default_height](/cells/sv/python-net/aspose.cells.charts/chartarea/default_height) | Representerar höjden på standardpositionen|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_position_auto()](/cells/sv/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Ställ in ramens position på automatisk|



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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [ChartArea](/cells/sv/python-net/aspose.cells.charts/chartarea)
* klass [ChartFrame](/cells/sv/python-net/aspose.cells.charts/chartframe)
* klass [Line](/cells/sv/python-net/aspose.cells.drawing/line)
