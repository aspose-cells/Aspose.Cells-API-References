---
title: calc_stack_size الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size الملكية

يحدد حجم المكدس لحساب الخلايا بشكل متكرر.
ستعطي القيمة الكبيرة لهذا الحجم أداءً أفضل عندما يكون هناك الكثير من الخلايا التي يجب حسابها بشكل متكرر.
من ناحية أخرى ، ستزيد القيمة الأكبر من مخاطر StackOverflowException.
إذا حصل المستخدم على StackOverflowException عند حساب الصيغ ، فيجب إنقاص هذه القيمة.

###  ملاحظات

ملاحظة: هذا العضو قد عفا عليه الزمن الآن. بدلاً من ذلك ، يرجى استخدام CalculationOptions
باستخدام CalcStackSize المحدد عند حساب الصيغ.
 ستتم إزالة هذا العقار بعد 12 شهرًا منذ فبراير 2022.
Aspose يعتذر عن أي إزعاج قد يكون سببه لك.
###  تعريف:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [WorkbookSettings](/cells/ar/python-net/aspose.cells/workbooksettings)
