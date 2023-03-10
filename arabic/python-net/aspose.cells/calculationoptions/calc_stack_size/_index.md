---
title: calc_stack_size الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size الملكية

يحدد حجم المكدس لحساب الخلايا بشكل متكرر.

###  ملاحظات

عندما يكون هناك عدد كبير من الخلايا يلزم حسابها بشكل متكرر في شجرة التبعية ،
قد يكون سبب StackOverflowException في عملية الحساب.
إذا كان الأمر كذلك ، يجب على المستخدم تحديد قيمة أصغر لهذه الخاصية.
في مثل هذه الحالة ، يجب على المستخدم تحديد القيمة المناسبة لهذه الخاصية وفقًا للصيغ والبيانات الفعلية.
قد تتسبب القيمة الصغيرة جدًا في تدهور الأداء لحساب الصيغة.
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
* فئة [CalculationOptions](/cells/ar/python-net/aspose.cells/calculationoptions)
