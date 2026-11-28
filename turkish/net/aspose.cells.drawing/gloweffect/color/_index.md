---
title: "GlowEffect.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlowEffect özelliği. Parıltı efektinin rengini alır"
type: docs
url: /tr/net/aspose.cells.drawing/gloweffect/color/
---
## GlowEffect.Color property

Parıltı etkisinin rengini alır.

```csharp
public CellsColor Color { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 100, 100, 100, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            
            CellsColor glowColor = shape.Glow.Color;
            glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


