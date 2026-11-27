---
title: "Shape.TextVerticalOverflow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger den vertikala översvämningstypen för texten i formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

Hämtar och anger den vertikala översvämningstypen för texten i formen som innehåller text.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // Ställ in text och låt den överflöda vertikalt
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // Spara arbetsboken
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


