---
title: "Shape.TextOrientationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger textorienteringstypen för formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Hämtar och anger textorienteringstypen för formen.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Ange text för formen
            shape.Text = "Sample Text";

            // Kontrollera och modifiera textorienteringen
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Spara arbetsboken
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


