---
title: "Range.RowCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient le nombre de lignes dans la plage"
type: docs
url: /fr/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Obtient le nombre de lignes dans la plage.

```csharp
public int RowCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez des données d'exemple dans les cellules A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Créez une plage nommée couvrant A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Obtenir la plage nommée
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Démontrer la propriété RowCount
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


