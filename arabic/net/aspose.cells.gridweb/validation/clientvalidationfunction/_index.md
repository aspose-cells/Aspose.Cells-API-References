---
title: "Validation.ClientValidationFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. يحصل أو يحدد اسم دالة جافاسكريبت للتحقق من صحة العميل"
type: docs
url: /ar/net/aspose.cells.gridweb/validation/clientvalidationfunction/
---
## Validation.ClientValidationFunction property

يحصل أو يعيّن اسم دالة جافاسكريبت للتحقق من صحة العميل.

```csharp
public string ClientValidationFunction { get; set; }
```

### ملاحظات

استخدم خاصية ClientValidationFunction لتحديد اسم دالة التحقق من صحة العميل. يجب إعلان الدالة بهذه الصيغة: function customValicationFunction(source, value) المعامل "source" هو كائن الخلية. المعامل "value" هو القيمة النصية للخلية التي سيتم فحصها. يجب أن تُعيد الدالة true إذا كانت القيمة صالحة.

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


