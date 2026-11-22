---
title: "GridValidation.GetListValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridValidation. الحصول على القيمة لقائمة التحقق من الصحة للخلية المحددة"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

احصل على القيمة لقائمة التحقق للخلية المحددة.

```csharp
public object GetListValue(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

القيمة لإنتاج قائمة هذا التحقق من الصحة للخلية المحددة. إذا كانت القائمة تشير إلى نطاق، فستكون القيمة المرجعة كائن ReferredArea؛ وإلا قد تكون القيمة المرجعة null أو object[] أو كائن بسيط.

### ملاحظات

فقط للتحقق الذي يكون نوعه List وتم تطبيقه على الخلية المعطاة، وإلا سيتم إرجاع null.

### انظر أيضًا

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


