---
title: "CellArea.EndColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Campo CellArea. Ottiene o imposta la colonna finale di quest'area"
type: docs
url: /it/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Ottiene o imposta la colonna finale di quest'area.

```csharp
public int EndColumn;
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea un'area di celle da A1 a C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Elabora l'area di celle usando EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Salva la cartella di lavoro
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

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


