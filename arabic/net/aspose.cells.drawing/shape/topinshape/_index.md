---
title: "Shape.TopInShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب بوحدة 1/4000 من ارتفاع الشكل الأب"
type: docs
url: /ar/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.

```csharp
public int TopInShape { get; set; }
```

### ملاحظات

يطبق فقط عندما يكون هذا الشكل داخل مجموعة أو مخطط.

### أمثلة

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


