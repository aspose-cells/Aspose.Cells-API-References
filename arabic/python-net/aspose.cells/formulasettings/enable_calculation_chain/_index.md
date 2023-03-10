---
title: enable_calculation_chain الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain الملكية

سواء تم تمكين سلسلة الحساب للصيغ. الافتراضي هو خطأ.

###  ملاحظات

عندما يكون هناك الكثير من الصيغ في المصنف ويحتاج المستخدم إلى حسابها بشكل متكرر
مع تعديل جزء صغير منها فقط ، قد يكون من المفيد للأداء تمكين سلسلة الحساب.
من ناحية أخرى ، إذا تم تمكين السلسلة ، فإن الحفاظ على نموذج السلسلة يتطلب ذاكرة إضافية ،
ويتطلب أيضًا وقتًا أكبر قليلاً في وحدة المعالجة المركزية لبعض العمليات الأخرى مثل تغيير قيمة الخلية أو الصيغ.
بعد تغيير هذه الخاصية من خطأ إلى صحيح ، سيتم تحليل وبناء سلسلة الحساب
في وقت الحساب الأول للمصنف ، وبالتالي الوقت المطلوب للحساب الأول
قد يكون أكثر من الحساب العادي بدون سلسلة.
###  تعريف:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [FormulaSettings](/cells/ar/python-net/aspose.cells/formulasettings)
