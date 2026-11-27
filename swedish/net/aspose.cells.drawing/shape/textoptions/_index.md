---
title: "Shape.TextOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar textalternativen för formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Representerar textalternativen för formen.

```csharp
public TextOptions TextOptions { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Ange text för formen
            shape.Text = "Sample Text";

            // Åtkomst och ändra TextOptions
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Spara arbetsboken
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


