---
title: "Shape.Spid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Anger en valfri strängidentifierare som en applikation kan använda för att identifiera den specifika shape"
type: docs
url: /sv/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Specificerar en valfri strängidentifierare som ett program kan använda för att identifiera den specifika formen.

```csharp
public string Spid { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelshape i arbetsbladet med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Hämta och visa Spid-egenskapen för shape
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Spara arbetsboken
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


