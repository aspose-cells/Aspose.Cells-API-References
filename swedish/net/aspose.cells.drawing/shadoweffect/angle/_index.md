---
title: "ShadowEffect.Angle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger belysningsvinkeln. Intervall från 0 till 359,9 grader"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Hämtar och anger belysningsvinkeln. Omfång från 0 till 359,9 grader.

```csharp
public double Angle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och ange skuggeffektens vinkel
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Verifiera och skriv ut vinkelvärdet
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


