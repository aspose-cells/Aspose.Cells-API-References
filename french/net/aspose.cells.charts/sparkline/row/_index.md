---
title: "Sparkline.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Sparkline. Obtient l'indice de ligne du sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Obtient l'indice de ligne du sparkline.

```csharp
public int Row { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Créer un groupe de sparkline
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Ajouter un sparkline à la ligne 0, colonne 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Afficher la position de la ligne (propriété en lecture seule)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Pour changer la position, nous devons supprimer et recréer le sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Enregistrer le classeur
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


