---
title: "Worksheet.CellWatches"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient la collection de cellules de cette feuille de calcul surveillées dans la fenêtre de surveillance"
type: docs
url: /fr/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Obtient la collection de cellules de cette feuille de calcul surveillées dans le 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la cellule B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Ajouter une surveillance de cellule pour B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Afficher les informations de surveillance
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Enregistrez le classeur
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


