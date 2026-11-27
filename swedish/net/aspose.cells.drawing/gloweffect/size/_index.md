---
title: "GlowEffect.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlowEffect-egenskap. Hämtar och anger radien för glow i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Hämtar och anger glödens radie i enheter av punkter.

```csharp
public double Size { get; set; }
```

### Exempel

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
            
            // Ställ in egenskaper för glödeffekten
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


