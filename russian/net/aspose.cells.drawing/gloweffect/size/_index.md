---
title: "GlowEffect.Size"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GlowEffect. Получает и задает радиус свечения в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Получает и задает радиус свечения в единицах пунктов.

```csharp
public double Size { get; set; }
```

### Примеры

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
            
            // Установить свойства эффекта свечения
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


