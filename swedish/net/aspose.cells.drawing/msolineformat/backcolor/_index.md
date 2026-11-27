---
title: "MsoLineFormat.BackColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat-egenskap. Hämtar och anger bakgrundsfärgen för kantlinjen"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Hämtar och anger kantlinjens bakgrundsfärg.

```csharp
public Color BackColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Ställ in linjeegenskaper
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Spara arbetsboken
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


