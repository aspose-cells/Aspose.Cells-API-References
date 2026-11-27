---
title: "Shape.TextHorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar och anger den horisontella justeringstypen för texten i formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Hämtar och anger den horisontella justeringstypen för texten i formen.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Ställ in text och justering
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Ändra justeringen om den för närvarande är Nederst
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Spara arbetsboken
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


