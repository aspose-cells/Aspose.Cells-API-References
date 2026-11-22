---
title: "GlowEffect.Radius"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlowEffect. تحصل وتضبط نصف قطر التوهج بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

الحصول على وتعيين نصف قطر التوهج، بوحدة النقاط.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية GlowEffect.Size. ستتم إزالة هذه الخاصية بعد 6 أشهر منذ سبتمبر 2016. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyRadiusDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
            arcShape.Placement = PlacementType.FreeFloating;
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = System.Drawing.Color.Blue;

            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = System.Drawing.Color.Yellow;
            glowEffect.Radius = 15.0; // Demonstrating Radius property
            glowEffect.Transparency = 0.3;

            workbook.Save("GlowEffectRadiusDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


