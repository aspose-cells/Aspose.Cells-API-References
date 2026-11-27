---
title: "MsoLineFormat.DashStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat-egenskap. Hämtar eller anger streckstilen för den angivna linjen"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Hämtar eller anger streckstilen för den angivna linjen.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till en form för att demonstrera DashStyle
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Ställ in linjeegenskaper
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // Demonstrera olika streckstilar
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // Lägg till en annan form med annan streckstil
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // Spara arbetsboken
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


