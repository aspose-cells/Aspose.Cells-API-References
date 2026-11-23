---
title: "Range.FirstColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient l'index de la première colonne de la plage"
type: docs
url: /fr/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Obtient l'index de la première colonne de la plage.

```csharp
public int FirstColumn { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Créez une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Démontrer la propriété FirstColumn
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Utiliser FirstColumn pour accéder aux cellules de la première colonne de la plage
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Enregistrez le classeur
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


