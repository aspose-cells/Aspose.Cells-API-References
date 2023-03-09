---
title: Line klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 290
url: /sv/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line klass
Kapslar in objektet som representerar linjeformatet.



Typen Line avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [compound_type](/cells/sv/python-net/aspose.cells.drawing/line/compound_type) |Anger den sammansatta linjetypen|
| [dash_type](/cells/sv/python-net/aspose.cells.drawing/line/dash_type) | Anger typen av strecklinje|
| [cap_type](/cells/sv/python-net/aspose.cells.drawing/line/cap_type) | Anger slutbeteckningarna.|
| [join_type](/cells/sv/python-net/aspose.cells.drawing/line/join_type) | Specificerar sammanfogningslocken.|
| [begin_type](/cells/sv/python-net/aspose.cells.drawing/line/begin_type) | Anger en pilspets för början av en rad.|
| [end_type](/cells/sv/python-net/aspose.cells.drawing/line/end_type) | Anger en pilspets för slutet av en rad.|
| [begin_arrow_length](/cells/sv/python-net/aspose.cells.drawing/line/begin_arrow_length) | Anger längden på pilspetsen för början av en linje.|
| [end_arrow_length](/cells/sv/python-net/aspose.cells.drawing/line/end_arrow_length) | Anger längden på pilspetsen för slutet av en linje.|
| [begin_arrow_width](/cells/sv/python-net/aspose.cells.drawing/line/begin_arrow_width) | Anger bredden på pilspetsen för början av en linje.|
| [end_arrow_width](/cells/sv/python-net/aspose.cells.drawing/line/end_arrow_width) | Anger bredden på pilspetsen för slutet av en linje.|
| [theme_color](/cells/sv/python-net/aspose.cells.drawing/line/theme_color) | Får och ställer in temafärgen.|
| [color](/cells/sv/python-net/aspose.cells.drawing/line/color) | Representerar färgen på linjen.|
| [transparency](/cells/sv/python-net/aspose.cells.drawing/line/transparency) | Returnerar eller ställer in graden av transparens för linjen som ett värde från 0,0 (opak) till 1,0 (ren).|
| [style](/cells/sv/python-net/aspose.cells.drawing/line/style) | Representerar linjens stil.|
| [weight](/cells/sv/python-net/aspose.cells.drawing/line/weight) | Hämtar eller ställer in linjens [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype).|
| [weight_pt](/cells/sv/python-net/aspose.cells.drawing/line/weight_pt) | Hämtar eller ställer in linjens vikt i poängenhet.|
| [weight_px](/cells/sv/python-net/aspose.cells.drawing/line/weight_px) | Hämtar eller ställer in linjens vikt i pixelenhet.|
| [formatting_type](/cells/sv/python-net/aspose.cells.drawing/line/formatting_type) | Hämtar eller ställer in formattyp.|
| [is_automatic_color](/cells/sv/python-net/aspose.cells.drawing/line/is_automatic_color) |Indikerar om färgen på linjen tilldelas automatiskt.|
| [is_visible](/cells/sv/python-net/aspose.cells.drawing/line/is_visible) | Representerar om linjen är synlig.|
| [is_auto](/cells/sv/python-net/aspose.cells.drawing/line/is_auto) | Indikerar om denna linjestil är autotilldelad.|
| [gradient_fill](/cells/sv/python-net/aspose.cells.drawing/line/gradient_fill) | Representerar gradientfyllning.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartMarkerType, ChartType
from aspose.cells.drawing import LineType, WeightType
from aspose.pydrawing import Color

workbook = Workbook()
sheet = workbook.worksheets[0]
cells = sheet.cells
cells.get(0, 1).put_value("Income")
cells.get(1, 0).put_value("Company A")
cells.get(2, 0).put_value("Company B")
cells.get(3, 0).put_value("Company C")
cells.get(1, 1).put_value(10000)
cells.get(2, 1).put_value(20000)
cells.get(3, 1).put_value(30000)
chartIndex = sheet.charts.add(ChartType.LINE, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
# Applying a dotted line style on the lines of an NSeries
chart.n_series[0].border.style = LineType.DOT
chart.n_series[0].border.color = Color.red
# Applying a triangular marker style on the data markers of an NSeries
chart.n_series[0].marker.marker_style = ChartMarkerType.TRIANGLE
# Setting the weight of all lines in an NSeries to medium
chart.n_series[0].border.weight = WeightType.MEDIUM_LINE

```

###  Se även
* modul [aspose.cells.drawing](..)
* klass [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype)
