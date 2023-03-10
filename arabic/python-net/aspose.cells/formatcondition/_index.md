---
title: FormatCondition الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 690
url: /ar/python-net/aspose.cells/formatcondition/
is_root: false
---
##  FormatCondition الدرجة
يمثل شرط التنسيق الشرطي.



يكشف نوع FormatCondition الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [formula1](/cells/ar/python-net/aspose.cells/formatcondition/formula1) | الحصول على القيمة أو التعبير المرتبط بالتنسيق الشرطي وتعيينهما.|
| [formula2](/cells/ar/python-net/aspose.cells/formatcondition/formula2) | الحصول على القيمة أو التعبير المرتبط بالتنسيق الشرطي وتعيينهما.|
| [operator](/cells/ar/python-net/aspose.cells/formatcondition/operator) | الحصول على نوع مشغل التنسيق الشرطي وتعيينه.|
| [stop_if_true](/cells/ar/python-net/aspose.cells/formatcondition/stop_if_true) |صحيح ، لا يمكن تطبيق أي قواعد ذات أولوية أقل على هذه القاعدة ، عندما يتم تقييم هذه القاعدة على صواب.<br/> ينطبق فقط على Excel 2007 ؛|
| [priority](/cells/ar/python-net/aspose.cells/formatcondition/priority) | أولوية قاعدة التنسيق الشرطي هذه. يتم استخدام هذه القيمة لتحديد أي<br/>يجب تقييم التنسيق وتقديمه. القيم الرقمية الأقل أولوية أعلى من<br/> القيم الرقمية الأعلى ، حيث يمثل "1" الأولوية القصوى.|
| [style](/cells/ar/python-net/aspose.cells/formatcondition/style) | الحصول على أو تحديد نمط نطاقات الخلايا المنسقة الشرطية.|
| [type](/cells/ar/python-net/aspose.cells/formatcondition/type) | الحصول على نوع التنسيق الشرطي وتحديده.|
| [icon_set](/cells/ar/python-net/aspose.cells/formatcondition/icon_set) | احصل على مثيل "IconSet" للتنسيق الشرطي.<br/>IconSetType للمثيل الافتراضي هو TrafficLights31.<br/> صالح فقط لنوع = IconSet.|
| [data_bar](/cells/ar/python-net/aspose.cells/formatcondition/data_bar) | احصل على مثيل "DataBar" الخاص بالتنسيق الشرطي.<br/>اللون الافتراضي للمثيل هو الأزرق.<br/> صالح فقط للنوع هو DataBar.|
| [color_scale](/cells/ar/python-net/aspose.cells/formatcondition/color_scale) | احصل على مثيل "ColorScale" الخاص بالتنسيق الشرطي.<br/>المثيل الافتراضي هو 3ColorScale "أخضر - أصفر - أحمر".<br/> صالح فقط للنوع = ColorScale.|
| [top10](/cells/ar/python-net/aspose.cells/formatcondition/top10) | احصل على مثيل "Top10" للتنسيق الشرطي.<br/>تبرز قاعدة المثيل الافتراضي الخلايا التي تحتوي على<br/>تقع القيم في أعلى 10 شريحة.<br/> صالح فقط للنوع هو Top10.|
| [above_average](/cells/ar/python-net/aspose.cells/formatcondition/above_average) |احصل على مثيل "AboveAverage" للتنسيق الشرطي.<br/> تقوم قاعدة المثيل الافتراضية بتمييز الخلايا الموجودة<br/>فوق المتوسط لجميع القيم في النطاق.<br/> صالح فقط لنوع = AboveAverage.|
| [text](/cells/ar/python-net/aspose.cells/formatcondition/text) | قيمة النص في "نص يحتوي على" قاعدة تنسيق شرطي.<br/>صالح فقط للنوع = يحتوي على نص ، لا يحتوي على نص ، يبدأ مع وينتهي.<br/> القيمه الافتراضيه فارغه.|
| [time_period](/cells/ar/python-net/aspose.cells/formatcondition/time_period) | الفترة الزمنية المطبقة في قاعدة التنسيق الشرطي "تاريخ حدوث ...".<br/>صالح فقط للنوع = timePeriod.<br/> القيمة الافتراضية هي TimePeriodType.Today.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | الحصول على القيمة أو التعبير المرتبط بشرط التنسيق هذا.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) | الحصول على قيمة أو تعبير التنسيق الشرطي للخلية.|
| [get_formula1(row, column)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | الحصول على صيغة التنسيق الشرطي للخلية.|
| [get_formula2(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | الحصول على القيمة أو التعبير المرتبط بشرط التنسيق هذا.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) | الحصول على قيمة أو تعبير التنسيق الشرطي للخلية.|
| [get_formula2(row, column)](/cells/ar/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | الحصول على صيغة التنسيق الشرطي للخلية.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | يعيّن القيمة أو التعبير المرتبط بشرط التنسيق هذا.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | يعيّن القيمة أو التعبير المرتبط بشرط التنسيق هذا.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | يعيّن القيمة أو التعبير المرتبط بشرط التنسيق هذا.|



###  مثال

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
