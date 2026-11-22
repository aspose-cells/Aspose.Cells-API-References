---
title: "Shape.Glow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثّل كائن GlowEffect الذي يحدد تأثير التوهج لعنصر المخطط أو الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

تمثّل كائن [`GlowEffect`](../../gloweffect/) الذي يحدد تأثير التوهج لعنصر المخطط أو الشكل.

```csharp
public GlowEffect Glow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // الوصول إلى تأثير التوهج
            GlowEffect glow = shape.Glow;

            // عيّن خصائص التوهج
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // احفظ المصنف
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


