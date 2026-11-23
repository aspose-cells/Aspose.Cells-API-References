---
title: "Series.HasDropLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Vrai si le graphique possède des lignes de chute. S'applique uniquement aux graphiques en ligne ou aux graphiques en aires"
type: docs
url: /fr/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

Vrai si le graphique possède des lignes de chute. S'applique uniquement aux graphiques en courbes ou aux graphiques en aires.

```csharp
public bool HasDropLines { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des données de série
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir la première série
            Series series = chart.NSeries[0];

            // Démontrer la propriété HasDropLines
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Enregistrez le classeur
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


