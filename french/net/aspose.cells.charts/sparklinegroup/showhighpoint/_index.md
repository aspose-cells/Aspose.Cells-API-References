---
title: "SparklineGroup.ShowHighPoint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Indique s'il faut mettre en évidence les points les plus élevés des données dans le groupe de sparkline."
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Indique s'il faut mettre en évidence les points les plus élevés de données dans le groupe de sparkline.

```csharp
public bool ShowHighPoint { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHighPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Créer un groupe de sparkline
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Ajouter un sparkline
            group.Sparklines.Add("A1:D1", 0, 4);

            // Configurer l'affichage du point haut
            group.ShowHighPoint = true;
            CellsColor highColor = workbook.CreateCellsColor();
            highColor.Color = System.Drawing.Color.Green;
            group.HighPointColor = highColor;

            // Enregistrer le classeur
            workbook.Save("SparklineHighPointDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


