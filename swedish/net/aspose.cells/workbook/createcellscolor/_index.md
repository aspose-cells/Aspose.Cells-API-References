---
title: "Workbook.CreateCellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Skapar ett CellsColor-objekt"
type: docs
url: /sv/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Skapar ett [`CellsColor`](../../cellscolor/) objekt.

```csharp
public CellsColor CreateCellsColor()
```

### Returvärde

Returnerar ett [`CellsColor`](../../cellscolor/) objekt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Skapa ett område och sätt kanter med anpassad färg
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Verifiera kantstilen i en specifik cell
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


