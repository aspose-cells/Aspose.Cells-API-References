---
title: FillFormat Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat Klasse
Kapselt das Objekt, das die Füllformatierung für eine Form darstellt.



Der Typ FillFormat macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [type](/cells/de/python-net/aspose.cells.drawing/fillformat/type) | Ruft den Fülltyp ab und legt ihn fest.|
| [fill_type](/cells/de/python-net/aspose.cells.drawing/fillformat/fill_type) | Ruft den Fülltyp ab und legt ihn fest|
| [transparency](/cells/de/python-net/aspose.cells.drawing/fillformat/transparency) | Gibt den Transparenzgrad des Bereichs als Wert von 0,0 (deckend) bis 1,0 (durchsichtig) zurück oder legt ihn fest.|
| [set_type](/cells/de/python-net/aspose.cells.drawing/fillformat/set_type) | Ruft den Typ des Füllformatsatzes ab.|
| [gradient_fill](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Ruft [FillFormat.gradient_fill](/cells/de/python-net/aspose.cells.drawing/fillformat#gradient_fill)-Objekt ab.|
| [texture_fill](/cells/de/python-net/aspose.cells.drawing/fillformat/texture_fill) | Ruft [FillFormat.texture_fill](/cells/de/python-net/aspose.cells.drawing/fillformat#texture_fill)-Objekt ab.|
| [solid_fill](/cells/de/python-net/aspose.cells.drawing/fillformat/solid_fill) | Ruft [FillFormat.solid_fill](/cells/de/python-net/aspose.cells.drawing/fillformat#solid_fill)-Objekt ab.|
| [pattern_fill](/cells/de/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Ruft [FillFormat.pattern_fill](/cells/de/python-net/aspose.cells.drawing/fillformat#pattern_fill)-Objekt ab.|
| [gradient_color_type](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Gibt den Verlaufsfarbtyp für die angegebene Füllung zurück.|
| [gradient_style](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_style) | Gibt den Verlaufsstil für die angegebene Füllung zurück.|
| [gradient_color1](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Gibt die Verlaufsfarbe 1 für die angegebene Füllung zurück.|
| [gradient_color2](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Gibt die Verlaufsfarbe 2 für die angegebene Füllung zurück.|
| [gradient_degree](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Gibt den Gradientengrad für die angegebene Füllung zurück.<br/> Gilt nur für Excel 2007.|
| [gradient_variant](/cells/de/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Gibt die Verlaufsvariante für die angegebene Füllung zurück.<br/> Gilt nur für Excel 2007.|
| [preset_color](/cells/de/python-net/aspose.cells.drawing/fillformat/preset_color) | Gibt die voreingestellte Verlaufsfarbe für die angegebene Füllung zurück.|
| [texture](/cells/de/python-net/aspose.cells.drawing/fillformat/texture) | Repräsentiert den Texturtyp für die angegebene Füllung.|
| [pattern](/cells/de/python-net/aspose.cells.drawing/fillformat/pattern) | Repräsentiert das Anzeigemuster eines Bereichs.|
| [picture_format_type](/cells/de/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Ruft den Bildformattyp ab und legt ihn fest.|
| [scale](/cells/de/python-net/aspose.cells.drawing/fillformat/scale) | Ruft die Bildformatskalierung ab und legt sie fest.|
| [image_data](/cells/de/python-net/aspose.cells.drawing/fillformat/image_data) | Ruft die Bilddaten ab und legt sie fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/de/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest.<br/> Gilt nur für Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/de/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest.<br/> Gilt nur für Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/de/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Legt die angegebene Füllung auf einen einfarbigen Farbverlauf fest.<br/> Gilt nur für Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/de/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Legt die angegebene Füllung auf einen voreingestellten Farbverlauf fest.<br/> Gilt nur für Excel 2007.|



###  Beispiel

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color

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
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)

```

###  Siehe auch
* Modul [aspose.cells.drawing](..)
