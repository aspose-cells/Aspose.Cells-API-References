---
title: "Shape.IsSmartArt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Anger om formen är en smart art"
type: docs
url: /sv/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Anger om formen är en smart art.

```csharp
public bool IsSmartArt { get; }
```

### Anmärkningar

Endast för ooxml-fil.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en SmartArt-form (Obs: Aspose.Cells exponerar inte direkt skapandet av SmartArt i nuvarande versioner)
            // För demonstration kommer vi att kontrollera befintliga former
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Kontrollera om formen är SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


