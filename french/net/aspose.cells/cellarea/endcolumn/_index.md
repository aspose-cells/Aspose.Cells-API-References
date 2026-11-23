---
title: "CellArea.EndColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Champ CellArea. Obtient ou définit la colonne de fin de cette zone"
type: docs
url: /fr/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Obtient ou définit la colonne de fin de cette zone.

```csharp
public int EndColumn;
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer une zone de cellules de A1 à C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Traiter la zone de cellules en utilisant EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Enregistrez le classeur
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

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


