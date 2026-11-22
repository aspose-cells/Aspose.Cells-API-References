---
title: "Shape.LeftInShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب بوحدة 1/4000 من عرض الشكل الأب"
type: docs
url: /ar/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب.

```csharp
public int LeftInShape { get; set; }
```

### ملاحظات

يطبق فقط عندما يكون هذا الشكل داخل مجموعة أو مخطط.

### أمثلة

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


