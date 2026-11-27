---
title: "CellsColor.Argb"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsColor property. Hämtar och anger färgen från ett 32-bit ARGB-värde"
type: docs
url: /sv/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Hämtar och sätter färgen från ett 32-bitars ARGB-värde.

```csharp
public int Argb { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område och en stil
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Skapa och konfigurera CellsColor med Argb property
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Applicera färgen på stilen
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Applicera stil på område
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Spara arbetsboken
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


