---
title: "طريقة SetCheckExcelRestriction"
linktitle: "SetCheckExcelRestriction"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "طريقة SetCheckExcelRestriction. تغلف الدالة التي تمثل setcheckexcelrestriction في Go."
type: docs
weight: 200
url: /ar/go-cpp/jsonloadoptions/setcheckexcelrestriction/
---

## SetCheckExcelRestriction function

ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة السلسلة التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

```go

func (instance *JsonLoadOptions) SetCheckExcelRestriction(value bool)  error

```

## ملاحظات


## انظر أيضًا

* Class [JsonLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
