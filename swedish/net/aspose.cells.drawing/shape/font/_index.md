---
title: "Shape.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Representerar formens teckensnitt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Representerar formens teckensnitt.

```csharp
public Font Font { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Åtkomst till och ändra teckensnittsegenskaperna för formen
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Spara arbetsboken
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


