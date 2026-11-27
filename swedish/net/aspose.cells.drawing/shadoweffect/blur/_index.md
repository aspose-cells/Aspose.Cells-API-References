---
title: "ShadowEffect.Blur"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger suddigheten för skuggan. Intervall från 0 till 100 punkter"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Hämtar och anger suddigheten för skuggan. Intervall från 0 till 100 punkter.

```csharp
public double Blur { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en exempelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Hämta skuggeffekt
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Ange skuggegenskaper inklusive Suddighet
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Se även

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


