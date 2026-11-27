---
title: "Shape.TextDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar/Sätter riktningen för textflödet för detta objekt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Hämtar/anger riktningen för textflödet för detta objekt.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Ställ in och demonstrera TextDirection-egenskapen
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Ändra textens riktning
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Spara arbetsboken
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


