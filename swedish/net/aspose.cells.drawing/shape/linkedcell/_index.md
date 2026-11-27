---
title: "Shape.LinkedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar eller anger kalkylbladsintervallet som är länkat till kontrollens värde"
type: docs
url: /sv/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Hämtar eller anger kalkylbladsintervallet som är länkat till kontrollens värde.

```csharp
public string LinkedCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ställ in LinkedCell‑egenskapen till B6
            shape.LinkedCell = "$B$6";

            // Ändra LinkedCell till A1 om den var B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Skriv ut det aktuella LinkedCell‑värdet
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


