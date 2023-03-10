---
title: calculation_mode الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 60
url: /ar/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode الملكية

الحصول على أو تحديد وضع حساب المصنف في ms excel.

###  ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج
بحيث تعمل التطبيقات الأخرى (مثل ms excel) وفقًا لذلك عند تحميل الملف الناتج ومعالجته.
للنظر في الأداء لمعظم تطبيقات المستخدم ، لا نقوم بحساب أي صيغة في المصنف تلقائيًا ،
بغض النظر عن الوضع الذي تم تعيينه لهذه الخاصية.
إذا احتاج المستخدم إلى حساب الصيغ ، فيرجى دائمًا استدعاء الطرق على كائنات مختلفة وفقًا للمتطلبات:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/ar/python-net/aspose.cells/cell/calculate)، ... إلخ.
###  تعريف:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [CalcModeType](/cells/ar/python-net/aspose.cells/calcmodetype)
* فئة [FormulaSettings](/cells/ar/python-net/aspose.cells/formulasettings)
