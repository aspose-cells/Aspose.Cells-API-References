---
title: "CellsColor.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsColor property. Hämtar och anger transparens som ett värde från 0.0 ogenomskinlig till 1.0 klar"
type: docs
url: /sv/net/aspose.cells/cellscolor/transparency/
---
## CellsColor.Transparency property

Hämtar och sätter transparens som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.FromArgb(128, 255, 0, 0); // Semi-transparent red
            cellsColor.Transparency = 0.5; // Set transparency to 50%

            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;

            worksheet.Cells["A1"].PutValue("50% transparent red background");
            worksheet.Cells["A1"].SetStyle(style);

            workbook.Save("TransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


