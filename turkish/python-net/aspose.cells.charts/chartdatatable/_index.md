---
title: ChartDataTable sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 60
url: /tr/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable sınıfı
Bir grafik veri tablosunu temsil eder.



ChartDataTable türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [font](/cells/tr/python-net/aspose.cells.charts/chartdatatable/font) | Belirtilen grafik veri tablosunun yazı tipi ayarını temsil eden bir [ChartDataTable.font](/cells/tr/python-net/aspose.cells.charts/chartdatatable#font) nesnesi alır.|
| [auto_scale_font](/cells/tr/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | Nesne boyutu değiştiğinde, nesnedeki metin yazı tipi boyutunu değiştirirse doğrudur.<br/> Varsayılan değer True'dur.|
| [background_mode](/cells/tr/python-net/aspose.cells.charts/chartdatatable/background_mode) | Arka planın görüntüleme modunu alır ve ayarlar|
| [background](/cells/tr/python-net/aspose.cells.charts/chartdatatable/background) | Arka planın görüntüleme modunu alır ve ayarlar|
| [has_border_horizontal](/cells/tr/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |Grafik veri tablosunun yatay hücre kenarlıkları varsa doğrudur|
| [has_border_vertical](/cells/tr/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | Grafik veri tablosunun dikey hücre kenarlıkları varsa doğrudur|
| [has_border_outline](/cells/tr/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | Grafik veri tablosunda ana hat kenarlıkları varsa doğrudur|
| [show_legend_key](/cells/tr/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | Veri etiketi gösterge anahtarı görünüyorsa doğrudur.|
| [border](/cells/tr/python-net/aspose.cells.charts/chartdatatable/border) | Nesnenin kenarlığını temsil eden bir Border nesnesi döndürür|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
