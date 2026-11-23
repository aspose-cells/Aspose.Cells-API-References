---
title: "Row.Index"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient l'index de cette ligne"
type: docs
url: /fr/net/aspose.cells/row/index/
---
## Row.Index property

Obtient l'index de cette ligne.

```csharp
public int Index { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Itérer à travers les lignes et démontrer la propriété Index
            foreach (Row row in worksheet.Cells.Rows)
            {
                Console.WriteLine($"Processing row with index: {row.Index}");
                if (row.Index > 0) // Skip header row
                {
                    Console.WriteLine($"Data in row {row.Index}: " +
                        $"{worksheet.Cells[row.Index, 0].StringValue}, " +
                        $"{worksheet.Cells[row.Index, 1].IntValue}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


