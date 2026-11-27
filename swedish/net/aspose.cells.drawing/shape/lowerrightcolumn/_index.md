---
title: "Shape.LowerRightColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar kolumnindex för nedre högra hörnet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lowerrightcolumn/
---
## Shape.LowerRightColumn property

Representerar kolumnindex för nedre högra hörnet.

```csharp
public int LowerRightColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Ställ in och visa det initiala LowerRightColumn‑värdet
            shape.LowerRightColumn = 3;
            Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);

            // Ändra LowerRightColumn om den är lika med 3
            if (shape.LowerRightColumn == 3)
            {
                shape.LowerRightColumn = 1;
                Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


