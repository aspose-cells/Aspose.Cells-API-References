---
title: AbstractCalculationMonitor الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor الدرجة
مراقبة للمستخدم لتتبع التقدم المحرز في حساب الصيغة.



يكشف نوع AbstractCalculationMonitor الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [original_value](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/original_value) | الحصول على القيمة القديمة للخلية المحسوبة.<br/> يجب استخدامه فقط في [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) و [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | ما إذا تم تغيير قيمة الخلية بعد الحساب أم لا.<br/> يجب استخدامه فقط في [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | الحصول على القيمة المحسوبة حديثًا للخلية.<br/> يجب استخدامه فقط في [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | قم بتنفيذ هذه الطريقة للقيام بالأعمال قبل حساب خلية واحدة.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | قم بتنفيذ هذه الطريقة لممارسة الأعمال التجارية بعد حساب خلية واحدة.|
| [on_circular(circular_cells_data)](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | قم بتنفيذ هذه الطريقة للقيام بالأعمال عند حساب الصيغ باستخدام مراجع دائرية.|



###  أنظر أيضا
* وحدة [aspose.cells](..)
