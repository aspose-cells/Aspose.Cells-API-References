---
title: "Shape.LeftCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar den horisontella förskjutningen av figuren från dess vänstra kolumn i enheten centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Representerar den horisontella förskjutningen av figuren från dess vänstra kolumn, i enhet centimeter.

```csharp
public double LeftCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in och hämta LeftCM‑egenskapen
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Ändra vänsterpositionen om den är 3 cm
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


