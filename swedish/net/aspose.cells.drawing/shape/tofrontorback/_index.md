---
title: "Shape.ToFrontOrBack"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Flyttar formen till framsidan eller skickar den till bak"
type: docs
url: /sv/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Flyttar formen framåt eller skickar den bakåt.

```csharp
public void ToFrontOrBack(int orders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ordningar | Int32 | Om den är mindre än noll, placeras formen i bakgrunden. Om den är större än noll, flyttas formen till framsidan. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till två former för att demonstrera z‑ordning
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Flytta shape2 två positioner framåt i z‑ordning
            shape2.ToFrontOrBack(2);

            // Flytta shape1 en position bakåt i z‑ordning
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


