---
title: "Sparkline.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Sparkline. Obtient l'index de colonne du sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Obtient l'indice de colonne du sparkline.

```csharp
public int Column { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
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
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Ajoutez un sparkline à la colonne 4 et démontrez la propriété Column
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Affichez la propriété column (lecture seule)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // Pour changer la position de la colonne, nous devons supprimer et réajouter le sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Enregistrer le classeur
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


