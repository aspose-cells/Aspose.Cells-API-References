---
title: "Range.SetInsideBorders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Ställ in innermarginaler för området"
type: docs
url: /sv/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Ställ in inre kanter för området.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | BorderType | Typ av innermarginal, kan bara vara Vertikal och Horisontell. |
| lineStyle | CellBorderType | Marginalstilen. |
| borderColor | CellsColor | Färgen på kantlinjen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område och ställ in innermarginaler
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Verifiera marginalerna i en cell inom området
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### Se även

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


