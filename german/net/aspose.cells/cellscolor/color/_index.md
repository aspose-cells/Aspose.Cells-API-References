---
title: "CellsColor.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor-Eigenschaft. Liest und setzt die RGB-Farbe"
type: docs
url: /de/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Liest und setzt die RGB‑Farbe.

```csharp
public Color Color { get; set; }
```

### Beispiele

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

            // Erstellen Sie einen Bereich und setzen Sie farbige Rahmen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Überprüfen Sie die Rahmen-Einstellungen in einer Zelle
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Speichere die Arbeitsmappe
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


