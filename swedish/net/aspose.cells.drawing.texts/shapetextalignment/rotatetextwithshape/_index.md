---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Anger om text roteras med formen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Anger om text roteras med formen.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textrutaform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Kom åt egenskaper för textjustering
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Ställ in RotateTextWithShape-egenskapen
            textAlignment.RotateTextWithShape = true;

            // Rotera formen för att demonstrera effekten
            shape.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


