---
title: ChartArea sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea sınıf
Çalışma sayfasındaki grafik alanını temsil eden nesneyi kapsüller.



**Miras:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/tr/python-net/aspose.cells.charts/chartframe)



ChartArea türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_inner_mode](/cells/tr/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Çizim alanı boyutunun, onay işaretlerini ve eksen etiketlerini içerip içermediğini gösterir.<br/> False, boyutun çizim alanının boyutunu, onay işaretlerini ve eksen etiketlerini belirleyeceğini belirtir.|
| [border](/cells/tr/python-net/aspose.cells.charts/chartarea/border) | [Line](/cells/tr/python-net/aspose.cells.drawing/line)'i alır.|
| [area](/cells/tr/python-net/aspose.cells.charts/chartarea/area) | [ChartFrame.area](/cells/tr/python-net/aspose.cells.charts/chartframe#area)'i alır.|
| [text_font](/cells/tr/python-net/aspose.cells.charts/chartarea/text_font) | Belirtilen ChartFrame nesnesinin [ChartFrame.font](/cells/tr/python-net/aspose.cells.charts/chartframe#font) nesnesini alır.|
| [text_options](/cells/tr/python-net/aspose.cells.charts/chartarea/text_options) | Metnin seçeneklerini alır ve ayarlar.|
| [font](/cells/tr/python-net/aspose.cells.charts/chartarea/font) | Belirtilen chartarea nesnesinin [ChartArea.font](/cells/tr/python-net/aspose.cells.charts/chartarea#font) nesnesini alır.|
| [auto_scale_font](/cells/tr/python-net/aspose.cells.charts/chartarea/auto_scale_font) | Nesne boyutu değiştiğinde, nesnedeki metin yazı tipi boyutunu değiştirirse doğrudur. Varsayılan değer True'dur.|
| [background_mode](/cells/tr/python-net/aspose.cells.charts/chartarea/background_mode) | Arka planın görüntüleme modunu alır ve ayarlar|
| [background](/cells/tr/python-net/aspose.cells.charts/chartarea/background) | Arka planın görüntüleme modunu alır ve ayarlar|
| [is_automatic_size](/cells/tr/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir.|
| [x](/cells/tr/python-net/aspose.cells.charts/chartarea/x) | Sol üst köşe sütunundan yatay uzaklığı alır veya alır.|
| [y](/cells/tr/python-net/aspose.cells.charts/chartarea/y) | Sol üst köşe satırından dikey uzaklığı alır veya alır.|
| [height](/cells/tr/python-net/aspose.cells.charts/chartarea/height) | Sağ alt köşe satırından dikey uzaklığı alır veya ayarlar.|
| [width](/cells/tr/python-net/aspose.cells.charts/chartarea/width) | Sağ alt köşe sütunundan yatay uzaklığı alır veya ayarlar.|
| [shadow](/cells/tr/python-net/aspose.cells.charts/chartarea/shadow) | Çerçevede gölge varsa doğrudur.|
| [shape_properties](/cells/tr/python-net/aspose.cells.charts/chartarea/shape_properties) | [ChartFrame.shape_properties](/cells/tr/python-net/aspose.cells.charts/chartframe#shape_properties) nesnesini alır.|
| [is_default_pos_be_set](/cells/tr/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir.|
| [default_x](/cells/tr/python-net/aspose.cells.charts/chartarea/default_x) | Varsayılan konumun x'ini temsil eder|
| [default_y](/cells/tr/python-net/aspose.cells.charts/chartarea/default_y) | Varsayılan konumun y'sini temsil eder|
| [default_width](/cells/tr/python-net/aspose.cells.charts/chartarea/default_width) | Varsayılan konumun genişliğini temsil eder|
| [default_height](/cells/tr/python-net/aspose.cells.charts/chartarea/default_height) | Varsayılan konumun yüksekliğini temsil eder|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_position_auto()](/cells/tr/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Çerçevenin konumunu otomatik olarak ayarlayın|



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

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [ChartArea](/cells/tr/python-net/aspose.cells.charts/chartarea)
* sınıf [ChartFrame](/cells/tr/python-net/aspose.cells.charts/chartframe)
* sınıf [Line](/cells/tr/python-net/aspose.cells.drawing/line)
