---
title: "Shape.Top"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar den vertikala förskjutningen av formen från dess översta rad i enhet pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Representerar figurens vertikala förskjutning från dess översta rad, i pixlar.

```csharp
public int Top { get; set; }
```

### Anmärkningar

Om formen är i diagrammet representerar den vertikala förskjutningen av formen från dess övre kant.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ange initial topposition
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Modifiera toppositionen om den är lika med 3 (demonstrerar testfallslogiken)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // För demonstration, sätt till 3 och tillämpa sedan testfallslogiken
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


