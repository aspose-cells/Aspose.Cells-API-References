---
title: Line الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 290
url: /ar/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line الدرجة
لتغليف الكائن الذي يمثل تنسيق الخط.



يكشف نوع Line الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [compound_type](/cells/ar/python-net/aspose.cells.drawing/line/compound_type) | يحدد نوع الخط المركب|
| [dash_type](/cells/ar/python-net/aspose.cells.drawing/line/dash_type) | يحدد نوع خط الشرطة|
| [cap_type](/cells/ar/python-net/aspose.cells.drawing/line/cap_type) | يحدد قبعات النهاية.|
| [join_type](/cells/ar/python-net/aspose.cells.drawing/line/join_type) | يحدد قبعات الانضمام.|
| [begin_type](/cells/ar/python-net/aspose.cells.drawing/line/begin_type) |يحدد رأس سهم لبداية السطر.|
| [end_type](/cells/ar/python-net/aspose.cells.drawing/line/end_type) | يحدد رأس سهم لنهاية السطر.|
| [begin_arrow_length](/cells/ar/python-net/aspose.cells.drawing/line/begin_arrow_length) | يحدد طول رأس السهم لبداية السطر.|
| [end_arrow_length](/cells/ar/python-net/aspose.cells.drawing/line/end_arrow_length) | يحدد طول رأس السهم لنهاية السطر.|
| [begin_arrow_width](/cells/ar/python-net/aspose.cells.drawing/line/begin_arrow_width) | يحدد عرض رأس السهم لبداية السطر.|
| [end_arrow_width](/cells/ar/python-net/aspose.cells.drawing/line/end_arrow_width) | يحدد عرض رأس السهم لنهاية السطر.|
| [theme_color](/cells/ar/python-net/aspose.cells.drawing/line/theme_color) | الحصول على لون المظهر وتعيينه.|
| [color](/cells/ar/python-net/aspose.cells.drawing/line/color) | يمثل لون الخط.|
| [transparency](/cells/ar/python-net/aspose.cells.drawing/line/transparency) | إرجاع أو تعيين درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (واضح).|
| [style](/cells/ar/python-net/aspose.cells.drawing/line/style) | يمثل نمط الخط.|
| [weight](/cells/ar/python-net/aspose.cells.drawing/line/weight) | الحصول على او تحديد [WeightType](/cells/ar/python-net/aspose.cells.drawing/weighttype) للخط.|
| [weight_pt](/cells/ar/python-net/aspose.cells.drawing/line/weight_pt) | الحصول على أو تحديد وزن الخط بوحدة النقاط.|
| [weight_px](/cells/ar/python-net/aspose.cells.drawing/line/weight_px) | الحصول على أو تحديد وزن الخط بوحدة البكسل.|
| [formatting_type](/cells/ar/python-net/aspose.cells.drawing/line/formatting_type) | يحصل أو يحدد نوع التنسيق.|
| [is_automatic_color](/cells/ar/python-net/aspose.cells.drawing/line/is_automatic_color) | يشير إلى ما إذا كان لون الخط معينًا تلقائيًا أم لا.|
| [is_visible](/cells/ar/python-net/aspose.cells.drawing/line/is_visible) | يمثل ما إذا كان الخط مرئيًا.|
| [is_auto](/cells/ar/python-net/aspose.cells.drawing/line/is_auto) | يشير إلى ما إذا كان نمط الخط هذا قد تم تعيينه تلقائيًا أم لا.|
| [gradient_fill](/cells/ar/python-net/aspose.cells.drawing/line/gradient_fill) | يمثل تعبئة متدرجة.|



###  مثال

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

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
* فئة [WeightType](/cells/ar/python-net/aspose.cells.drawing/weighttype)
