---
title: "Workbook.CreateCellsColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Erstellt ein CellsColor-Objekt"
type: docs
url: /de/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Erstellt ein [`CellsColor`](../../cellscolor/) Objekt.

```csharp
public CellsColor CreateCellsColor()
```

### Rückgabewert

Gibt ein [`CellsColor`](../../cellscolor/) Objekt zurück.

### Beispiele

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
            
            // Erstelle einen Bereich und setze Rahmen mit benutzerdefinierter Farbe
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Überprüfe den Rahmenstil in einer bestimmten Zelle
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

### Siehe auch

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


