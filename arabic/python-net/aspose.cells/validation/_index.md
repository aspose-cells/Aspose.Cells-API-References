---
title: Validation الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1540
url: /ar/python-net/aspose.cells/validation/
is_root: false
---
##  Validation الدرجة
يمثل التحقق من صحة البيانات.



يكشف نوع Validation الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [operator](/cells/ar/python-net/aspose.cells/validation/operator) | يمثل المشغل للتحقق من صحة البيانات.|
| [alert_style](/cells/ar/python-net/aspose.cells/validation/alert_style) | يمثل نمط تنبيه التحقق.|
| [type](/cells/ar/python-net/aspose.cells/validation/type) | يمثل نوع التحقق من صحة البيانات.|
| [input_message](/cells/ar/python-net/aspose.cells/validation/input_message) | يمثل رسالة إدخال التحقق من صحة البيانات.|
| [input_title](/cells/ar/python-net/aspose.cells/validation/input_title) | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات.|
| [error_message](/cells/ar/python-net/aspose.cells/validation/error_message) | يمثل رسالة خطأ التحقق من صحة البيانات.|
| [error_title](/cells/ar/python-net/aspose.cells/validation/error_title) | يمثل عنوان مربع حوار خطأ التحقق من صحة البيانات.|
| [show_input](/cells/ar/python-net/aspose.cells/validation/show_input) | يشير إلى ما إذا كان سيتم عرض رسالة إدخال التحقق من صحة البيانات عندما يحدد المستخدم خلية في نطاق التحقق من صحة البيانات.|
| [show_error](/cells/ar/python-net/aspose.cells/validation/show_error) | يشير إلى ما إذا كان سيتم عرض رسالة خطأ التحقق من صحة البيانات عندما يقوم المستخدم بإدخال بيانات غير صالحة.|
| [ignore_blank](/cells/ar/python-net/aspose.cells/validation/ignore_blank) | يشير إلى ما إذا كانت القيم الفارغة مسموحًا بها من خلال التحقق من صحة بيانات النطاق.|
| [formula1](/cells/ar/python-net/aspose.cells/validation/formula1) | يمثل القيمة أو التعبير المرتبط بالتحقق من صحة البيانات.|
| [formula2](/cells/ar/python-net/aspose.cells/validation/formula2) | يمثل القيمة أو التعبير المرتبط بالتحقق من صحة البيانات.|
| [value1](/cells/ar/python-net/aspose.cells/validation/value1) | يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات.|
| [value2](/cells/ar/python-net/aspose.cells/validation/value2) | يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات.|
| [in_cell_drop_down](/cells/ar/python-net/aspose.cells/validation/in_cell_drop_down) | يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على قيم مقبولة.|
| [areas](/cells/ar/python-net/aspose.cells/validation/areas) | يحصل على جميع [CellArea](/cells/ar/python-net/aspose.cells/cellarea) التي تحتوي على إعدادات التحقق من صحة البيانات.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/validation/get_formula1/#bool-bool) | الحصول على القيمة أو التعبير المرتبط بهذا التحقق من الصحة.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/ar/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق من الصحة لخلية معينة.|
| [get_formula2(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/validation/get_formula2/#bool-bool) | الحصول على القيمة أو التعبير المرتبط بهذا التحقق من الصحة.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/ar/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق من الصحة لخلية معينة.|
| [add_area(cell_area)](/cells/ar/python-net/aspose.cells/validation/add_area/#CellArea) | يطبق التحقق على المنطقة.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/ar/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | يطبق التحقق على المنطقة.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | يعيّن القيمة أو التعبير المرتبط بعملية التحقق هذه.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | يعيّن القيمة أو التعبير المرتبط بعملية التحقق هذه.|
| [get_list_value(row, column)](/cells/ar/python-net/aspose.cells/validation/get_list_value/#int-int) |احصل على قيمة قائمة التحقق من صحة الخلية المحددة.|
| [add_areas(areas, check_intersection, check_edge)](/cells/ar/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | يطبق التحقق على مناطق معينة.|
| [remove_area(cell_area)](/cells/ar/python-net/aspose.cells/validation/remove_area/#CellArea) | قم بإزالة إعدادات التحقق من الصحة في النطاق.|
| [remove_areas(areas)](/cells/ar/python-net/aspose.cells/validation/remove_areas/#list) | يزيل هذا التحقق من الصحة من مناطق معينة.|
| [remove_a_cell(row, column)](/cells/ar/python-net/aspose.cells/validation/remove_a_cell/#int-int) | قم بإزالة إعدادات التحقق من الصحة في الخلية.|
| [copy(source, copy_option)](/cells/ar/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | التحقق من النسخ.|



###  مثال

```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [CellArea](/cells/ar/python-net/aspose.cells/cellarea)
