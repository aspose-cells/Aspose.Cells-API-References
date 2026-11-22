---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GridWorkbookSettings. ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الخلايا أو الكائنات المرتبطة. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K مثلًا عبر Cell.PutValuestring إذا كانت هذه الخاصية true ستحصل على استثناء. إذا كانت الخاصية false سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك إذا قمت بتعيين قيمة من هذا النوع غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ دفتر العمل بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. القيمة الافتراضية هي false.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### انظر أيضًا

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


