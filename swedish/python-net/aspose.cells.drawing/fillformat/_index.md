---
title: FillFormat klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat klass
Kapslar in objektet som representerar fyllningsformatering för en form.



Typen FillFormat avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [type](/cells/sv/python-net/aspose.cells.drawing/fillformat/type) |Hämtar och ställer in fyllningstypen.|
| [fill_type](/cells/sv/python-net/aspose.cells.drawing/fillformat/fill_type) | Hämtar och ställer in fyllningstyp|
| [transparency](/cells/sv/python-net/aspose.cells.drawing/fillformat/transparency) | Returnerar eller ställer in graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (ren).|
| [set_type](/cells/sv/python-net/aspose.cells.drawing/fillformat/set_type) | Hämtar uppsättningstypen för fyllningsformat.|
| [gradient_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Får [FillFormat.gradient_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat#gradient_fill) objekt.|
| [texture_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat/texture_fill) | Får [FillFormat.texture_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat#texture_fill) objekt.|
| [solid_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat/solid_fill) | Får [FillFormat.solid_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat#solid_fill) objekt.|
| [pattern_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Får [FillFormat.pattern_fill](/cells/sv/python-net/aspose.cells.drawing/fillformat#pattern_fill) objekt.|
| [gradient_color_type](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Returnerar gradientfärgtypen för den angivna fyllningen.|
| [gradient_style](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_style) | Returnerar gradientstilen för den angivna fyllningen.|
| [gradient_color1](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Returnerar gradientfärg 1 för den angivna fyllningen.|
| [gradient_color2](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Returnerar gradientfärg 2 för den angivna fyllningen.|
| [gradient_degree](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Returnerar gradientgraden för den angivna fyllningen.<br/> Gäller endast Excel 2007.|
| [gradient_variant](/cells/sv/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Returnerar gradientvarianten för den angivna fyllningen.<br/> Gäller endast Excel 2007.|
| [preset_color](/cells/sv/python-net/aspose.cells.drawing/fillformat/preset_color) | Returnerar den förinställda övertoningsfärgen för den angivna fyllningen.|
| [texture](/cells/sv/python-net/aspose.cells.drawing/fillformat/texture) | Representerar texturtypen för den angivna fyllningen.|
| [pattern](/cells/sv/python-net/aspose.cells.drawing/fillformat/pattern) | Representerar ett områdes visningsmönster.|
| [picture_format_type](/cells/sv/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Hämtar och ställer in bildformatstyp.|
| [scale](/cells/sv/python-net/aspose.cells.drawing/fillformat/scale) | Hämtar och ställer in bildformatsskalan.|
| [image_data](/cells/sv/python-net/aspose.cells.drawing/fillformat/image_data) | Hämtar och ställer in bildbildsdata.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/sv/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Ställer in den angivna fyllningen till en tvåfärgsgradient.<br/> Gäller endast Excel 2007.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/sv/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Ställer in den angivna fyllningen till en tvåfärgsgradient.<br/> Gäller endast Excel 2007.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/sv/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Ställer in den angivna fyllningen till en enfärgsgradient.<br/> Gäller endast Excel 2007.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/sv/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Ställer in den angivna fyllningen till en förinställd färggradient.<br/> Gäller endast Excel 2007.|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](..)
