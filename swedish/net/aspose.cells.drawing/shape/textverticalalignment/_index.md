---
title: "Shape.TextVerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar och anger den vertikala justeringstypen för texten i shape"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

Hämtar och anger den vertikala justeringstypen för texten i formen.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Ställ in text och justering
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // Ändra vertikal justering
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // Spara arbetsboken
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


