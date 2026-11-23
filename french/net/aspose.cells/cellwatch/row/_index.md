---
title: "CellWatch.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellWatch. Obtient et définit la ligne de la cellule"
type: docs
url: /fr/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Obtient et définit la ligne de la cellule.

```csharp
public int Row { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la cellule B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Ajoutez un CellWatch pour B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Démontrez la propriété Row
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Vérifiez la référence de la cellule
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


