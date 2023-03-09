---
title: Trendline klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 330
url: /sv/python-net/aspose.cells.charts/trendline/
is_root: false
---
##  Trendline klass
Representerar en trendlinje i ett diagram.



**Arv:** [Trendline](/cells/python-net/aspose.cells.charts/trendline) → 
[Line](/cells/sv/python-net/aspose.cells.drawing/line)



Typen Trendline avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [compound_type](/cells/sv/python-net/aspose.cells.charts/trendline/compound_type) | Anger den sammansatta linjetypen|
| [dash_type](/cells/sv/python-net/aspose.cells.charts/trendline/dash_type) | Anger typen av strecklinje|
| [cap_type](/cells/sv/python-net/aspose.cells.charts/trendline/cap_type) | Anger slutbeteckningarna.|
| [join_type](/cells/sv/python-net/aspose.cells.charts/trendline/join_type) | Specificerar sammanfogningslocken.|
| [begin_type](/cells/sv/python-net/aspose.cells.charts/trendline/begin_type) |Anger en pilspets för början av en rad.|
| [end_type](/cells/sv/python-net/aspose.cells.charts/trendline/end_type) | Anger en pilspets för slutet av en rad.|
| [begin_arrow_length](/cells/sv/python-net/aspose.cells.charts/trendline/begin_arrow_length) | Anger längden på pilspetsen för början av en linje.|
| [end_arrow_length](/cells/sv/python-net/aspose.cells.charts/trendline/end_arrow_length) | Anger längden på pilspetsen för slutet av en linje.|
| [begin_arrow_width](/cells/sv/python-net/aspose.cells.charts/trendline/begin_arrow_width) | Anger bredden på pilspetsen för början av en linje.|
| [end_arrow_width](/cells/sv/python-net/aspose.cells.charts/trendline/end_arrow_width) | Anger bredden på pilspetsen för slutet av en linje.|
| [theme_color](/cells/sv/python-net/aspose.cells.charts/trendline/theme_color) | Får och ställer in temafärgen.|
| [color](/cells/sv/python-net/aspose.cells.charts/trendline/color) | Representerar färgen på linjen.|
| [transparency](/cells/sv/python-net/aspose.cells.charts/trendline/transparency) | Returnerar eller ställer in graden av transparens för linjen som ett värde från 0,0 (opak) till 1,0 (ren).|
| [style](/cells/sv/python-net/aspose.cells.charts/trendline/style) | Representerar linjens stil.|
| [weight](/cells/sv/python-net/aspose.cells.charts/trendline/weight) | Hämtar eller ställer in linjens [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype).|
| [weight_pt](/cells/sv/python-net/aspose.cells.charts/trendline/weight_pt) | Hämtar eller ställer in linjens vikt i poängenhet.|
| [weight_px](/cells/sv/python-net/aspose.cells.charts/trendline/weight_px) | Hämtar eller ställer in linjens vikt i pixelenhet.|
| [formatting_type](/cells/sv/python-net/aspose.cells.charts/trendline/formatting_type) | Hämtar eller ställer in formattyp.|
| [is_automatic_color](/cells/sv/python-net/aspose.cells.charts/trendline/is_automatic_color) | Indikerar om färgen på linjen tilldelas automatiskt.|
| [is_visible](/cells/sv/python-net/aspose.cells.charts/trendline/is_visible) | Representerar om linjen är synlig.|
| [is_auto](/cells/sv/python-net/aspose.cells.charts/trendline/is_auto) | Indikerar om denna linjestil är autotilldelad.|
| [gradient_fill](/cells/sv/python-net/aspose.cells.charts/trendline/gradient_fill) | Representerar gradientfyllning.|
| [is_name_auto](/cells/sv/python-net/aspose.cells.charts/trendline/is_name_auto) | Returnerar om Microsoft Excel bestämmer automatiskt namnet på trendlinjen.|
| [type](/cells/sv/python-net/aspose.cells.charts/trendline/type) | Returnerar trendlinjetypen.|
| [name](/cells/sv/python-net/aspose.cells.charts/trendline/name) | Returnerar namnet på trendlinjen.|
| [order](/cells/sv/python-net/aspose.cells.charts/trendline/order) | Returnerar eller ställer in trendlinjeordningen (ett heltal större än 1) när trendlinjetypen är polynom.<br/> Beställningen måste vara mellan 2 och 6.|
| [period](/cells/sv/python-net/aspose.cells.charts/trendline/period) | Returnerar eller ställer in perioden för trendlinjen för glidande medelvärde.|
| [forward](/cells/sv/python-net/aspose.cells.charts/trendline/forward) | Returnerar eller ställer in antalet perioder (eller enheter på ett punktdiagram) som trendlinjen sträcker sig framåt.<br/> Antalet perioder måste vara större än eller lika med noll.|
| [backward](/cells/sv/python-net/aspose.cells.charts/trendline/backward) | Returnerar eller ställer in antalet perioder (eller enheter på ett punktdiagram) som trendlinjen sträcker sig bakåt.<br/>Antalet perioder måste vara större än eller lika med noll.<br/> Om diagramtypen är kolumn måste antalet perioder vara mellan 0 och 0,5|
| [display_equation](/cells/sv/python-net/aspose.cells.charts/trendline/display_equation) |Representerar om ekvationen för trendlinjen visas i diagrammet (i samma dataetikett som R-kvadratvärdet).|
| [display_r_squared](/cells/sv/python-net/aspose.cells.charts/trendline/display_r_squared) | Representerar om trendlinjens R-kvadratvärde visas i diagrammet (i samma dataetikett som ekvationen). Om du ställer in den här egenskapen på True aktiveras dataetiketter automatiskt.|
| [intercept](/cells/sv/python-net/aspose.cells.charts/trendline/intercept) | Returnerar eller ställer in punkten där trendlinjen korsar värdeaxeln.|
| [data_labels](/cells/sv/python-net/aspose.cells.charts/trendline/data_labels) | Representerar DataLabels-objektet för den angivna serien.|
| [legend_entry](/cells/sv/python-net/aspose.cells.charts/trendline/legend_entry) | Får legendposten enligt denna trendlinje|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType

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
# adding a linear trendline
index = chart.n_series[0].trend_lines.add(TrendlineType.LINEAR)
trendline = chart.n_series[0].trend_lines[index]
# Setting the custom name of the trendline.
trendline.name = "Linear"
# Displaying the equation on chart
trendline.display_equation = True
# Displaying the R-Squared value on chart
trendline.display_r_squared = True
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells.charts](..)
* klass [Line](/cells/sv/python-net/aspose.cells.drawing/line)
* klass [Trendline](/cells/sv/python-net/aspose.cells.charts/trendline)
* klass [WeightType](/cells/sv/python-net/aspose.cells.drawing/weighttype)
