---
title: "Klass ShadowEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShadowEffect-klass. Denna klass specificerar skuggeffekten för diagramelementet eller formen"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Denna klass specificerar skuggeffekten för diagramelementet eller formen.

```csharp
public class ShadowEffect
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Hämtar och anger belysningsvinkeln. Omfång från 0 till 359,9 grader. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Hämtar och anger suddigheten för skuggan. Intervall från 0 till 100 punkter. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Hämtar och anger färgen på skuggan. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Hämtar och anger avståndet för skuggan. Intervall från 0 till 200 punkter. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Hämtar och anger den förinställda skuggtypen för skuggan. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Hämtar och anger storleken på skuggan. Intervall från 0 till 2,0. Meningslöst i inre skugga. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Hämtar och anger graden av transparens för skuggan. Intervall från 0,0 (opak) till 1,0 (klar). |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Hämta skuggeffekten för formen
            ShadowEffect shadow = shape.ShadowEffect;

            // Ställ in skuggegenskaper
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


