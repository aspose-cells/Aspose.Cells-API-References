---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Hämtar och anger rotationen för formen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Hämtar och anger rotationen för formen.

```csharp
public double RotationAngle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Ange formtext
            shape.Text = "Rotated Text";
            
            // Åtkomst till textjustering och ställ in rotationsvinkeln
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Spara arbetsboken
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


