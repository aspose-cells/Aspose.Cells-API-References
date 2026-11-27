---
title: "ShadowEffect.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger storleken på skuggan. Intervall från 0 till 2,0. Meningslöst i inre skugga"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Hämtar och anger storleken på skuggan. Intervall från 0 till 2,0. Meningslöst i inre skugga.

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
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook book = new Workbook();
            
            // Öppna första kalkylbladet och lägg till en form
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Hämta skuggeffekten och ange egenskaper inklusive Storlek
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Spara arbetsboken
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Se även

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


