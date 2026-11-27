---
title: "ShadowEffect.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger graden av transparens för skuggan. Intervall från 0.0 opakt till 1.0 transparent"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Hämtar och anger graden av transparens för skuggan. Intervall från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en form för att demonstrera skuggeffekt
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Hämta skuggeffekt och ange egenskaper inklusive Transparens
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Spara arbetsboken
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### Se även

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


