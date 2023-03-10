---
title: check_excel_restriction الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction الملكية

ما إذا كان التحقق من تقييد ملف Excel عند تعديل المستخدم للكائنات ذات الصلة بالخلايا.
على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت.
عند إدخال قيمة أطول من 32 كيلو بايت مثل Cell.PutValue (سلسلة) ، إذا كانت هذه الخاصية صحيحة ، فستحصل على استثناء.
إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية حتى يتم ذلك لاحقًا
يمكنك إخراج قيمة السلسلة الكاملة لتنسيقات ملفات أخرى مثل CSV.
ومع ذلك ، إذا قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ،
يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه.
###  تعريف:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [AbstractTextLoadOptions](/cells/ar/python-net/aspose.cells/abstracttextloadoptions)
