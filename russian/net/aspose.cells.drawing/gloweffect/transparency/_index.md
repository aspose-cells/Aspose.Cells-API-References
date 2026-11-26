---
title: "GlowEffect.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlowEffect. Получает и задает степень прозрачности эффекта свечения. Диапазон от 0,0 (непрозрачно) до 1,0 (полностью прозрачно)"
type: docs
url: /ru/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Получает и задает степень прозрачности эффекта свечения. Диапазон от 0.0 (непрозрачно) до 1.0 (прозрачно).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 10, 0, 10, 200, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            
            CellsColor glowColor = shape.Glow.Color;
            glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            wb.Save("output/glow_transparency_demo.xlsx");
        }
    }
}
```

### См. также

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


