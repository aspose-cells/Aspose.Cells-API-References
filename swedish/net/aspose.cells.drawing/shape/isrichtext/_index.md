---
title: "Shape.IsRichText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Anger om texten är rich text eller inte"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Om texten är rik text eller inte.

```csharp
public bool IsRichText { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med text
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Kontrollera om texten är rich text
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


