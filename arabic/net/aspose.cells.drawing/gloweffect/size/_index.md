---
title: "GlowEffect.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlowEffect. تحصل وتضبط نصف قطر التوهج بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

الحصول على وتعيين نصف قطر التوهج، بوحدة النقاط.

```csharp
public double Size { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 200, 100, 200, 100);
            
            // تعيين خصائص تأثير التوهج
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


