---
title: "CellArea.EndColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-fält. Hämtar eller anger slutkolumnen för detta område"
type: docs
url: /sv/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Hämtar eller anger slutkolumnen för detta område.

```csharp
public int EndColumn;
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa ett cellområde från A1 till C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Bearbeta cellområdet med EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Spara arbetsboken
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

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


