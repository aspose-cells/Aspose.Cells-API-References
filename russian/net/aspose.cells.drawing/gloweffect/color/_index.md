---
title: "GlowEffect.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlowEffect. Получает цвет свечения"
type: docs
url: /ru/net/aspose.cells.drawing/gloweffect/color/
---
## GlowEffect.Color property

Получает цвет эффекта свечения.

```csharp
public CellsColor Color { get; set; }
```

### Примеры

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

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


