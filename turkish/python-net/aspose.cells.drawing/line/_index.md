---
title: Line sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 290
url: /tr/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line sınıf
Çizgi biçimini temsil eden nesneyi kapsüller.



Line türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [compound_type](/cells/tr/python-net/aspose.cells.drawing/line/compound_type) |Bileşik çizgi tipini belirtir|
| [dash_type](/cells/tr/python-net/aspose.cells.drawing/line/dash_type) | Kısa çizgi tipini belirtir|
| [cap_type](/cells/tr/python-net/aspose.cells.drawing/line/cap_type) | Bitiş büyük harflerini belirtir.|
| [join_type](/cells/tr/python-net/aspose.cells.drawing/line/join_type) | Birleştirme büyük harflerini belirtir.|
| [begin_type](/cells/tr/python-net/aspose.cells.drawing/line/begin_type) | Bir satırın başlangıcı için bir ok başı belirtir.|
| [end_type](/cells/tr/python-net/aspose.cells.drawing/line/end_type) | Bir satırın sonu için bir ok başı belirtir.|
| [begin_arrow_length](/cells/tr/python-net/aspose.cells.drawing/line/begin_arrow_length) | Bir satırın başlangıcı için ok ucunun uzunluğunu belirtir.|
| [end_arrow_length](/cells/tr/python-net/aspose.cells.drawing/line/end_arrow_length) | Bir satırın sonu için ok ucunun uzunluğunu belirtir.|
| [begin_arrow_width](/cells/tr/python-net/aspose.cells.drawing/line/begin_arrow_width) | Bir satırın başlangıcı için ok ucunun genişliğini belirtir.|
| [end_arrow_width](/cells/tr/python-net/aspose.cells.drawing/line/end_arrow_width) | Bir satırın sonu için ok ucunun genişliğini belirtir.|
| [theme_color](/cells/tr/python-net/aspose.cells.drawing/line/theme_color) | Tema rengini alır ve ayarlar.|
| [color](/cells/tr/python-net/aspose.cells.drawing/line/color) | Çizginin Rengini temsil eder.|
| [transparency](/cells/tr/python-net/aspose.cells.drawing/line/transparency) | Çizginin şeffaflık derecesini 0,0 (opak) ila 1,0 (açık) arasında bir değer olarak döndürür veya ayarlar.|
| [style](/cells/tr/python-net/aspose.cells.drawing/line/style) | Çizginin stilini temsil eder.|
| [weight](/cells/tr/python-net/aspose.cells.drawing/line/weight) | Satırın [WeightType](/cells/tr/python-net/aspose.cells.drawing/weighttype)'ini alır veya ayarlar.|
| [weight_pt](/cells/tr/python-net/aspose.cells.drawing/line/weight_pt) | Nokta birimi cinsinden çizginin ağırlığını alır veya ayarlar.|
| [weight_px](/cells/tr/python-net/aspose.cells.drawing/line/weight_px) | Çizginin ağırlığını piksel birimi cinsinden alır veya ayarlar.|
| [formatting_type](/cells/tr/python-net/aspose.cells.drawing/line/formatting_type) | Biçim türünü alır veya ayarlar.|
| [is_automatic_color](/cells/tr/python-net/aspose.cells.drawing/line/is_automatic_color) |Çizgi renginin otomatik olarak atanıp atanmadığını gösterir.|
| [is_visible](/cells/tr/python-net/aspose.cells.drawing/line/is_visible) | Çizginin görünür olup olmadığını temsil eder.|
| [is_auto](/cells/tr/python-net/aspose.cells.drawing/line/is_auto) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir.|
| [gradient_fill](/cells/tr/python-net/aspose.cells.drawing/line/gradient_fill) | Degrade dolguyu temsil eder.|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
* sınıf [WeightType](/cells/tr/python-net/aspose.cells.drawing/weighttype)
