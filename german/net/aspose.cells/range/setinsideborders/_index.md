---
title: "Range.SetInsideBorders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Innenränder des Bereichs festlegen"
type: docs
url: /de/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Setzt innere Rahmen des Bereichs.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | BorderType | Innenrandtyp, kann nur Vertikal und Horizontal sein. |
| lineStyle | CellBorderType | Der Randstil. |
| borderColor | CellsColor | Die Farbe des Randes. |

### Beispiele

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

            // Erstelle einen Bereich und lege Innenränder fest
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Überprüfe die Ränder in einer Zelle innerhalb des Bereichs
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

### Siehe auch

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


