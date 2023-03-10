---
title: ErrorBar sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 150
url: /tr/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  ErrorBar sınıfı
Veri serisinin hata çubuğunu temsil eder.



**Miras:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/tr/python-net/aspose.cells.drawing/line)



ErrorBar türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [compound_type](/cells/tr/python-net/aspose.cells.charts/errorbar/compound_type) | Bileşik çizgi tipini belirtir|
| [dash_type](/cells/tr/python-net/aspose.cells.charts/errorbar/dash_type) | Kısa çizgi tipini belirtir|
| [cap_type](/cells/tr/python-net/aspose.cells.charts/errorbar/cap_type) | Bitiş büyük harflerini belirtir.|
| [join_type](/cells/tr/python-net/aspose.cells.charts/errorbar/join_type) | Birleştirme büyük harflerini belirtir.|
| [begin_type](/cells/tr/python-net/aspose.cells.charts/errorbar/begin_type) |Bir satırın başlangıcı için bir ok başı belirtir.|
| [end_type](/cells/tr/python-net/aspose.cells.charts/errorbar/end_type) | Bir satırın sonu için bir ok başı belirtir.|
| [begin_arrow_length](/cells/tr/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Bir satırın başlangıcı için ok ucunun uzunluğunu belirtir.|
| [end_arrow_length](/cells/tr/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Bir satırın sonu için ok ucunun uzunluğunu belirtir.|
| [begin_arrow_width](/cells/tr/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Bir satırın başlangıcı için ok ucunun genişliğini belirtir.|
| [end_arrow_width](/cells/tr/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Bir satırın sonu için ok ucunun genişliğini belirtir.|
| [theme_color](/cells/tr/python-net/aspose.cells.charts/errorbar/theme_color) | Tema rengini alır ve ayarlar.|
| [color](/cells/tr/python-net/aspose.cells.charts/errorbar/color) | Çizginin Rengini temsil eder.|
| [transparency](/cells/tr/python-net/aspose.cells.charts/errorbar/transparency) | Çizginin şeffaflık derecesini 0,0 (opak) ila 1,0 (açık) arasında bir değer olarak döndürür veya ayarlar.|
| [style](/cells/tr/python-net/aspose.cells.charts/errorbar/style) | Çizginin stilini temsil eder.|
| [weight](/cells/tr/python-net/aspose.cells.charts/errorbar/weight) | Satırın [WeightType](/cells/tr/python-net/aspose.cells.drawing/weighttype)'ini alır veya ayarlar.|
| [weight_pt](/cells/tr/python-net/aspose.cells.charts/errorbar/weight_pt) | Nokta birimi cinsinden çizginin ağırlığını alır veya ayarlar.|
| [weight_px](/cells/tr/python-net/aspose.cells.charts/errorbar/weight_px) | Çizginin ağırlığını piksel birimi cinsinden alır veya ayarlar.|
| [formatting_type](/cells/tr/python-net/aspose.cells.charts/errorbar/formatting_type) | Biçim türünü alır veya ayarlar.|
| [is_automatic_color](/cells/tr/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Çizgi renginin otomatik olarak atanıp atanmadığını gösterir.|
| [is_visible](/cells/tr/python-net/aspose.cells.charts/errorbar/is_visible) | Çizginin görünür olup olmadığını temsil eder.|
| [is_auto](/cells/tr/python-net/aspose.cells.charts/errorbar/is_auto) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir.|
| [gradient_fill](/cells/tr/python-net/aspose.cells.charts/errorbar/gradient_fill) | Degrade dolguyu temsil eder.|
| [type](/cells/tr/python-net/aspose.cells.charts/errorbar/type) |Hata çubuğu miktar türünü temsil eder.|
| [display_type](/cells/tr/python-net/aspose.cells.charts/errorbar/display_type) | Hata çubuğu görüntüleme tipini temsil eder.|
| [amount](/cells/tr/python-net/aspose.cells.charts/errorbar/amount) | Hata çubuğunun miktarını temsil eder.<br/> Tutar sıfırdan büyük veya sıfıra eşit olmalıdır.|
| [show_marker_t_top](/cells/tr/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Biçimlendirme hata çubuklarının bir T-top ile olup olmadığını gösterir.|
| [plus_value](/cells/tr/python-net/aspose.cells.charts/errorbar/plus_value) | Hata çubuğu türü Özel olduğunda pozitif hata miktarını temsil eder.|
| [minus_value](/cells/tr/python-net/aspose.cells.charts/errorbar/minus_value) | Hata çubuğu türü Özel olduğunda negatif hata miktarını temsil eder.|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [ErrorBar](/cells/tr/python-net/aspose.cells.charts/errorbar)
* sınıf [Line](/cells/tr/python-net/aspose.cells.drawing/line)
* sınıf [WeightType](/cells/tr/python-net/aspose.cells.drawing/weighttype)
