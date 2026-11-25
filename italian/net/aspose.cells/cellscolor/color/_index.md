---
title: "CellsColor.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Ottiene e imposta il colore RGB"
type: docs
url: /it/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Ottiene e imposta il colore RGB.

```csharp
public Color Color { get; set; }
```

### Esempi

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

            // Crea un intervallo e imposta bordi colorati
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Verifica le impostazioni del bordo in una cella
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Salva la cartella di lavoro
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


