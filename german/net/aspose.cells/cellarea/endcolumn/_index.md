---
title: "CellArea.EndColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellArea-Feld. Ruft die Endspalte dieses Bereichs ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Liest oder setzt die Endspalte dieses Bereichs.

```csharp
public int EndColumn;
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstellen Sie einen Zellbereich von A1 bis C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Verarbeiten Sie den Zellbereich mit EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Speichere die Arbeitsmappe
            workbook.Save("CellAreaFieldEndColumnDemo_output.xlsx");
        }

        private static void ProcessCellArea(CellArea area, Color color, Worksheet sheet)
        {
            int k = 0;
            for (int col = area.StartColumn; col <= area.EndColumn; col++)
            {
                for (int row = area.StartRow; row <= area.EndRow; row++)
                {
                    Cell cell = sheet.Cells[row, col];
                    
                    if (!color.IsEmpty)
                    {
                        Style style = cell.GetStyle();
                        style.ForegroundColor = color;
                        style.Pattern = BackgroundType.Solid;
                        cell.SetStyle(style);
                    }
                    
                    cell.PutValue(row + col + k);
                    k++;
                }
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


