---
title: "GlowEffect.Radius"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlowEffect. Получает и задает радиус свечения в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Получает и задает радиус свечения в единицах пунктов.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство GlowEffect.Size. Это свойство будет удалено через 6 месяцев, начиная с сентября 2016 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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

### См. также

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


