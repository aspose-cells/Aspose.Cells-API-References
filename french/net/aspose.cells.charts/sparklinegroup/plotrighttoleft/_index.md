---
title: "SparklineGroup.PlotRightToLeft"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Indique si les données du tracé sont de droite à gauche"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/plotrighttoleft/
---
## SparklineGroup.PlotRightToLeft property

Indique si les données du tracé sont de droite à gauche.

```csharp
public bool PlotRightToLeft { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotRightToLeftDemo
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
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ajouter un sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Définir les couleurs des sparklines
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Démontrer la propriété PlotRightToLeft
            group.PlotRightToLeft = true; // Plot data points from right to left

            // Enregistrez le classeur
            workbook.Save("SparklineRightToLeftDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


