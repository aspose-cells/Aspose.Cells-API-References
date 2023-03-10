---
title: FillFormat sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 180
url: /tr/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
##  FillFormat sınıfı
Bir şekil için dolgu biçimlendirmesini temsil eden nesneyi kapsüller.



FillFormat türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [type](/cells/tr/python-net/aspose.cells.drawing/fillformat/type) |Doldurma türünü alır ve ayarlar.|
| [fill_type](/cells/tr/python-net/aspose.cells.drawing/fillformat/fill_type) | Doldurma türünü alır ve ayarlar|
| [transparency](/cells/tr/python-net/aspose.cells.drawing/fillformat/transparency) | Alanın şeffaflık derecesini 0,0 (opak) ila 1,0 (temiz) arasında bir değer olarak döndürür veya ayarlar.|
| [set_type](/cells/tr/python-net/aspose.cells.drawing/fillformat/set_type) | Dolgu formatı set tipini alır.|
| [gradient_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_fill) | [FillFormat.gradient_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat#gradient_fill) nesnesini alır.|
| [texture_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat/texture_fill) | [FillFormat.texture_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat#texture_fill) nesnesini alır.|
| [solid_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat/solid_fill) | [FillFormat.solid_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat#solid_fill) nesnesini alır.|
| [pattern_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat/pattern_fill) | [FillFormat.pattern_fill](/cells/tr/python-net/aspose.cells.drawing/fillformat#pattern_fill) nesnesini alır.|
| [gradient_color_type](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Belirtilen dolgu için degrade renk türünü döndürür.|
| [gradient_style](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_style) | Belirtilen dolgu için degrade stilini döndürür.|
| [gradient_color1](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Belirtilen dolgu için degrade rengi 1'i döndürür.|
| [gradient_color2](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Belirtilen dolgu için degrade rengi 2'yi döndürür.|
| [gradient_degree](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Belirtilen dolgu için gradyan derecesini döndürür.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [gradient_variant](/cells/tr/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Belirtilen dolgu için gradyan değişkenini döndürür.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [preset_color](/cells/tr/python-net/aspose.cells.drawing/fillformat/preset_color) | Belirtilen dolgu için degrade ön ayar rengini döndürür.|
| [texture](/cells/tr/python-net/aspose.cells.drawing/fillformat/texture) | Belirtilen dolgu için doku tipini temsil eder.|
| [pattern](/cells/tr/python-net/aspose.cells.drawing/fillformat/pattern) | Bir alanın görüntüleme modelini temsil eder.|
| [picture_format_type](/cells/tr/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Resim biçimi türünü alır ve ayarlar.|
| [scale](/cells/tr/python-net/aspose.cells.drawing/fillformat/scale) | Resim biçimi ölçeğini alır ve ayarlar.|
| [image_data](/cells/tr/python-net/aspose.cells.drawing/fillformat/image_data) | Resim görüntü verilerini alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/tr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/tr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [set_one_color_gradient(color, degree, style, variant)](/cells/tr/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) | Belirtilen dolguyu tek renkli bir degradeye ayarlar.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/tr/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) | Belirtilen dolguyu önceden ayarlanmış bir renk gradyanına ayarlar.<br/> Yalnızca Excel 2007 için geçerlidir.|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
