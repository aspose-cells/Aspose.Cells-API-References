---
title: ChartDataTable الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 60
url: /ar/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable الدرجة
يمثل جدول بيانات الرسم البياني.



يكشف نوع ChartDataTable الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [font](/cells/ar/python-net/aspose.cells.charts/chartdatatable/font) | الحصول على عنصر [ChartDataTable.font](/cells/ar/python-net/aspose.cells.charts/chartdatatable#font) والذي يمثل محددات الخط لجدول بيانات المخطط المحدد.|
| [auto_scale_font](/cells/ar/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | صواب إذا كان النص في الكائن يغير حجم الخط عندما يتغير حجم الكائن.<br/> القيمة الافتراضية هي الحقيقية.|
| [background_mode](/cells/ar/python-net/aspose.cells.charts/chartdatatable/background_mode) | الحصول على وضبط وضع عرض الخلفية|
| [background](/cells/ar/python-net/aspose.cells.charts/chartdatatable/background) | الحصول على وضبط وضع عرض الخلفية|
| [has_border_horizontal](/cells/ar/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |صواب إذا كان جدول بيانات المخطط يحتوي على حدود خلية أفقية|
| [has_border_vertical](/cells/ar/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | صواب إذا كان جدول بيانات المخطط يحتوي على حدود خلية عمودية|
| [has_border_outline](/cells/ar/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | صواب إذا كان جدول بيانات المخطط يحتوي على حدود خارجية|
| [show_legend_key](/cells/ar/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | صواب إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا.|
| [border](/cells/ar/python-net/aspose.cells.charts/chartdatatable/border) | إرجاع كائن حد يمثل حد الكائن|



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

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
