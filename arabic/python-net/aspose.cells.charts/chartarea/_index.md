---
title: ChartArea الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea الدرجة
لتغليف الكائن الذي يمثل منطقة المخطط في ورقة العمل.



**ميراث:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/ar/python-net/aspose.cells.charts/chartframe)



يكشف نوع ChartArea الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_inner_mode](/cells/ar/python-net/aspose.cells.charts/chartarea/is_inner_mode) | يشير إلى ما إذا كان حجم مساحة الرسم يتضمن علامات التجزئة وتسميات المحور.<br/> تحدد False أن الحجم يجب أن يحدد حجم مساحة قطعة الأرض وعلامات التجزئة وتسميات المحور.|
| [border](/cells/ar/python-net/aspose.cells.charts/chartarea/border) | يحصل على [Line](/cells/ar/python-net/aspose.cells.drawing/line).|
| [area](/cells/ar/python-net/aspose.cells.charts/chartarea/area) | يحصل على [ChartFrame.area](/cells/ar/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/ar/python-net/aspose.cells.charts/chartarea/text_font) | الحصول على عنصر [ChartFrame.font](/cells/ar/python-net/aspose.cells.charts/chartframe#font) لعنصر ChartFrame المحدد.|
| [text_options](/cells/ar/python-net/aspose.cells.charts/chartarea/text_options) | الحصول على خيارات النص وتعيينها.|
| [font](/cells/ar/python-net/aspose.cells.charts/chartarea/font) | يحصل على كائن [ChartArea.font](/cells/ar/python-net/aspose.cells.charts/chartarea#font) من كائن المخطط المحدد.|
| [auto_scale_font](/cells/ar/python-net/aspose.cells.charts/chartarea/auto_scale_font) | صواب إذا كان النص في الكائن يغير حجم الخط عندما يتغير حجم الكائن. القيمة الافتراضية هي الحقيقية.|
| [background_mode](/cells/ar/python-net/aspose.cells.charts/chartarea/background_mode) | الحصول على وضبط وضع عرض الخلفية|
| [background](/cells/ar/python-net/aspose.cells.charts/chartarea/background) | الحصول على وضبط وضع عرض الخلفية|
| [is_automatic_size](/cells/ar/python-net/aspose.cells.charts/chartarea/is_automatic_size) | يشير إلى ما إذا كان حجم إطار المخطط تلقائيًا أم لا.|
| [x](/cells/ar/python-net/aspose.cells.charts/chartarea/x) | الحصول على أو الحصول على الإزاحة الأفقية من عمود الزاوية اليسرى العليا.|
| [y](/cells/ar/python-net/aspose.cells.charts/chartarea/y) |الحصول على أو الحصول على الإزاحة الرأسية من صف الزاوية اليسرى العليا.|
| [height](/cells/ar/python-net/aspose.cells.charts/chartarea/height) | الحصول على أو تحديد الإزاحة الرأسية من صف الزاوية اليمنى السفلية.|
| [width](/cells/ar/python-net/aspose.cells.charts/chartarea/width) | الحصول على أو ضبط الإزاحة الأفقية من عمود الزاوية اليمنى السفلي.|
| [shadow](/cells/ar/python-net/aspose.cells.charts/chartarea/shadow) | صحيح إذا كان للإطار ظل.|
| [shape_properties](/cells/ar/python-net/aspose.cells.charts/chartarea/shape_properties) | الحصول على كائن [ChartFrame.shape_properties](/cells/ar/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/ar/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | يشير إلى ما إذا كان قد تم تعيين الموضع الافتراضي (DefaultX و DefaultY و DefaultWidth و DefaultHeight).|
| [default_x](/cells/ar/python-net/aspose.cells.charts/chartarea/default_x) | يمثل س من الوضع الافتراضي|
| [default_y](/cells/ar/python-net/aspose.cells.charts/chartarea/default_y) | يمثل y الوضع الافتراضي|
| [default_width](/cells/ar/python-net/aspose.cells.charts/chartarea/default_width) | يمثل عرض الموضع الافتراضي|
| [default_height](/cells/ar/python-net/aspose.cells.charts/chartarea/default_height) | يمثل ارتفاع الموضع الافتراضي|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_position_auto()](/cells/ar/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | اضبط موضع الإطار على تلقائي|



###  مثال

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

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
* فئة [ChartArea](/cells/ar/python-net/aspose.cells.charts/chartarea)
* فئة [ChartFrame](/cells/ar/python-net/aspose.cells.charts/chartframe)
* فئة [Line](/cells/ar/python-net/aspose.cells.drawing/line)
