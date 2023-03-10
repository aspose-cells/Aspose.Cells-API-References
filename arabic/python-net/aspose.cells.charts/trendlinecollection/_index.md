---
title: TrendlineCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 340
url: /ar/python-net/aspose.cells.charts/trendlinecollection/
is_root: false
---
##  TrendlineCollection الدرجة
يمثل مجموعة من كل العناصر [Trendline](/cells/ar/python-net/aspose.cells.charts/trendline) لسلسلة البيانات المحددة.



يكشف نوع TrendlineCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(type)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType) | يقوم باضافة عنصر [Trendline](/cells/ar/python-net/aspose.cells.charts/trendline) لهذه المجموعة بالنوع المحدد.|
| [add(type, name)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/add/#TrendlineType-str) | يقوم باضافة عنصر [Trendline](/cells/ar/python-net/aspose.cells.charts/trendline) لهذه المجموعة بالنوع والاسم المحددين.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/index_of/#Trendline-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#Trendline-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.charts/trendlinecollection/binary_search/#Trendline) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
worksheet.cells.get("A1").put_value(50)
worksheet.cells.get("A2").put_value(100)
worksheet.cells.get("A3").put_value(150)
worksheet.cells.get("A4").put_value(200)
worksheet.cells.get("B1").put_value(60)
worksheet.cells.get("B2").put_value(32)
worksheet.cells.get("B3").put_value(50)
worksheet.cells.get("B4").put_value(40)
# Adding a chart to the worksheet
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 3, 3, 15, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:a3", True)
chart.n_series[0].trend_lines.add(TrendlineType.LINEAR, "MyTrendLine")
line = chart.n_series[0].trend_lines[0]
line.display_equation = True
line.display_r_squared = True
line.color = Color.red

```

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
* فئة [Trendline](/cells/ar/python-net/aspose.cells.charts/trendline)
