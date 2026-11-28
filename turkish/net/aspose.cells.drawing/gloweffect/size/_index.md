---
title: "GlowEffect.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlowEffect özelliği. Parıltının yarıçapını nokta biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Parıltının yarıçapını alır ve ayarlar, birim olarak puan cinsinden.

```csharp
public double Size { get; set; }
```

### Örnekler

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
            
            // Parıltı efekti özelliklerini ayarla
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


