---
title: "CellsColor-egenskap. Hämtar och anger RGB‑färgen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Skapa ett område och ange färgade kanter"
type: docs
url: /sv/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Hämtar och sätter RGB-färgen.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verifiera kantinställningarna i en cell
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // CellsColor.SetTintOfShapeColor
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Spara arbetsboken
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


