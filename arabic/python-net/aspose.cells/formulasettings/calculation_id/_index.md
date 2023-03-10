---
title: calculation_id الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id الملكية

يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف.

###  ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج
بحيث تعمل التطبيقات الأخرى (مثل ms excel) وفقًا لذلك عند تحميل الملف الناتج ومعالجته.
في حالة ms excel ، إذا كانت قيمة هذه الخاصية أقل من معرف محرك إعادة الحساب المرتبط
مع التطبيق الذي يفتح الملف الناتج ، سيعيد التطبيق حساب نتائج جميع الصيغ
في هذا المصنف مباشرة بعد تحميل الملف.
للنظر في الأداء لمعظم تطبيقات المستخدمين ، لا نقوم بحساب أي صيغة في المصنف تلقائيًا ،
بغض النظر عن القيمة التي تم تحديدها لهذه الخاصية.
###  تعريف:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [FormulaSettings](/cells/ar/python-net/aspose.cells/formulasettings)
