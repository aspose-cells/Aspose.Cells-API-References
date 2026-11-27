---
title: "SolidFill.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SolidFill-egenskap. Hämtar eller anger färgen"
type: docs
url: /sv/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Hämtar eller anger färgen.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet med korrekta parametrar
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Ange formegenskaper med färg
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Demonstrera användning av Color-egenskapen
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Spara arbetsboken
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


