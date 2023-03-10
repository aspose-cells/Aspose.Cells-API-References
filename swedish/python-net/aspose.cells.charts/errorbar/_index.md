---
title: ErrorBar klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 150
url: /sv/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  ErrorBar klass
Representerar felfältet för dataserien.



**Arv:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/sv/python-net/aspose.cells.drawing/line)



Typen ErrorBar avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [compound_type](/cells/sv/python-net/aspose.cells.charts/errorbar/compound_type) | Anger den sammansatta linjetypen|
| [dash_type](/cells/sv/python-net/aspose.cells.charts/errorbar/dash_type) | Anger typen av strecklinje|
| [cap_type](/cells/sv/python-net/aspose.cells.charts/errorbar/cap_type) | Anger slutbeteckningarna.|
| [join_type](/cells/sv/python-net/aspose.cells.charts/errorbar/join_type) | Specificerar sammanfogningslocken.|
| [begin_type](/cells/sv/python-net/aspose.cells.charts/errorbar/begin_type) |Anger en pilspets för början av en rad.|
| [end_type](/cells/sv/python-net/aspose.cells.charts/errorbar/end_type) | Anger en pilspets för slutet av en rad.|
| [begin_arrow_length](/cells/sv/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Anger längden på pilspetsen för början av en linje.|
| [end_arrow_length](/cells/sv/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Anger längden på pilspetsen för slutet av en linje.|
| [begin_arrow_width](/cells/sv/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Anger bredden på pilspetsen för början av en linje.|
| [end_arrow_width](/cells/sv/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Anger bredden på pilspetsen för slutet av en linje.|
| [theme_color](/cells/sv/python-net/aspose.cells.charts/errorbar/theme_color) | Får och ställer in temafärgen.|
| [color](/cells/sv/python-net/aspose.cells.charts/errorbar/color) | Representerar färgen på linjen.|
| [transparency](/cells/sv/python-net/aspose.cells.charts/errorbar/transparency) | Returnerar eller ställer in graden av transparens för linjen som ett värde från 0,0 (opak) till 1,0 (ren).|
| [style](/cells/sv/python-net/aspose.cells.charts/errorbar/style) | Representerar linjens stil.|
| [weight](/cells/sv/python-net/aspose.cells.charts/errorbar/weight) | Hämtar eller ställer in linjens [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype).|
| [weight_pt](/cells/sv/python-net/aspose.cells.charts/errorbar/weight_pt) | Hämtar eller ställer in linjens vikt i poängenhet.|
| [weight_px](/cells/sv/python-net/aspose.cells.charts/errorbar/weight_px) | Hämtar eller ställer in linjens vikt i pixelenhet.|
| [formatting_type](/cells/sv/python-net/aspose.cells.charts/errorbar/formatting_type) | Hämtar eller ställer in formattyp.|
| [is_automatic_color](/cells/sv/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Indikerar om färgen på linjen tilldelas automatiskt.|
| [is_visible](/cells/sv/python-net/aspose.cells.charts/errorbar/is_visible) | Representerar om linjen är synlig.|
| [is_auto](/cells/sv/python-net/aspose.cells.charts/errorbar/is_auto) | Indikerar om denna linjestil är autotilldelad.|
| [gradient_fill](/cells/sv/python-net/aspose.cells.charts/errorbar/gradient_fill) | Representerar gradientfyllning.|
| [type](/cells/sv/python-net/aspose.cells.charts/errorbar/type) |Representerar felstapelmängdstyp.|
| [display_type](/cells/sv/python-net/aspose.cells.charts/errorbar/display_type) | Representerar visningstyp för felfält.|
| [amount](/cells/sv/python-net/aspose.cells.charts/errorbar/amount) | Representerar mängden felfält.<br/> Beloppet måste vara större än eller lika med noll.|
| [show_marker_t_top](/cells/sv/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Indikerar om formateringsfelstaplar med en T-top.|
| [plus_value](/cells/sv/python-net/aspose.cells.charts/errorbar/plus_value) | Representerar positivt felmängd när felstapeltypen är anpassad.|
| [minus_value](/cells/sv/python-net/aspose.cells.charts/errorbar/minus_value) | Representerar negativt felbelopp när felstapeltypen är anpassad.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.NSeries)):
    aseries = chart.n_series[i]
    aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
    aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
    aseries.y_error_bar.amount = 5

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [ErrorBar](/cells/sv/python-net/aspose.cells.charts/errorbar)
* klass [Line](/cells/sv/python-net/aspose.cells.drawing/line)
* klass [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype)
