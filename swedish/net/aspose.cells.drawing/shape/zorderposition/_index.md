---
title: "Shape.ZOrderPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Returnerar positionen för en figur i z‑ordningen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Returnerar positionen för en form i z-ordningen.

```csharp
public int ZOrderPosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till tre figurer för att demonstrera ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // Ställ in ZOrder‑positioner
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // Ändra ZOrder för shape3 för att föra den till framkant
            shape3.ZOrderPosition = 0;

            // Spara arbetsboken
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


