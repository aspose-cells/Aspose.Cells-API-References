---
title: Floor الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 160
url: /ar/python-net/aspose.cells.charts/floor/
is_root: false
---
##  Floor الدرجة
لتغليف الكائن الذي يمثل أرضية مخطط ثلاثي الأبعاد.



**ميراث:** [Floor](/cells/python-net/aspose.cells.charts/floor) → 
[Area](/cells/ar/python-net/aspose.cells.drawing/area)



يكشف نوع Floor الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [background_color](/cells/ar/python-net/aspose.cells.charts/floor/background_color) | الحصول على او تحديد لون خلفية [Area](/cells/ar/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/ar/python-net/aspose.cells.charts/floor/foreground_color) | الحصول على او تحديد لون المقدمة.|
| [formatting](/cells/ar/python-net/aspose.cells.charts/floor/formatting) | يمثل تنسيق المنطقة.|
| [invert_if_negative](/cells/ar/python-net/aspose.cells.charts/floor/invert_if_negative) | إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط رقمًا سالبًا ،<br/> سيتم استبدال لون المقدمة ولون الخلفية.|
| [fill_format](/cells/ar/python-net/aspose.cells.charts/floor/fill_format) | يمثل عنصر [Area.fill_format](/cells/ar/python-net/aspose.cells.drawing/area#fill_format) يحتوي على خصائص تنسيق التعبئة للشكل أو الرسم البياني المحدد.|
| [transparency](/cells/ar/python-net/aspose.cells.charts/floor/transparency) | إرجاع أو تعيين درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (واضح).|
| [border](/cells/ar/python-net/aspose.cells.charts/floor/border) | الحصول على او تحديد الحدود [Line](/cells/ar/python-net/aspose.cells.drawing/line).|



###  مثال

```python
from aspose.cells import License, Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientPresetType, GradientStyleType
from aspose.pydrawing import Color

# Instantiate the License class
license = License()
# Pass only the name of the license file embedded in the assembly
license.set_license("Aspose.Cells.lic")
# Instantiate the workbook object
workbook = Workbook()
# Get cells collection
cells = workbook.worksheets[0].cells
# Put values in cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
cells.get("A3").put_value(3)
# get charts colletion
charts = workbook.worksheets[0].charts
# add a new chart
index = charts.add(ChartType.COLUMN_3D_STACKED, 5, 0, 15, 5)
# get the newly added chart
chart = charts[index]
# set charts nseries
chart.n_series.add("A1:A3", True)
# Show data labels
chart.n_series[0].data_labels.show_value = True
# Get chart's floor
floor = chart.floor
# set floor's border as red
floor.border.color = Color.red
# set fill format
floor.fill_format.set_preset_color_gradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2)
# save the file
workbook.save(r"dest.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
* فئة [Area](/cells/ar/python-net/aspose.cells.drawing/area)
* فئة [Floor](/cells/ar/python-net/aspose.cells.charts/floor)
* فئة [Line](/cells/ar/python-net/aspose.cells.drawing/line)
