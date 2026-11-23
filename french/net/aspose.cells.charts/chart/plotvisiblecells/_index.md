---
title: "Chart.PlotVisibleCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Indique si l’on ne trace que les cellules visibles"
type: docs
url: /fr/net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Indique si l’on ne trace que les cellules visibles.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété PlotVisibleCellsOnly. Cette méthode sera supprimée 12 mois plus tard depuis décembre 2022. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["A4"].PutValue("Eve");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(90);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(95);

            // Masquer certaines lignes
            worksheet.Cells.HideRow(2);
            worksheet.Cells.HideRow(3);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer la propriété PlotVisibleCells
            chart.PlotVisibleCells = false; // Will not plot hidden cells
            // chart.PlotVisibleCells = true; // Tracera les cellules cachées (commenté pour la démo)

            // Enregistrez le classeur
            workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


