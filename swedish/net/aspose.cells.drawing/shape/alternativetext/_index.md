---
title: "Shape.AlternativeText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Returnerar eller anger den beskrivande alternativa textsträngen för Shape-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Returnerar eller anger den beskrivande (alternativa) textsträngen för [`Shape`](../)-objektet.

```csharp
public string AlternativeText { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ange alternativ text för formen
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Spara arbetsboken
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


