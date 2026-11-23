---
title: "Line.WeightPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Obtient ou définit le poids de la ligne en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

Obtient ou définit le poids de la ligne en points.

```csharp
public double WeightPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer les étiquettes de données
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.HasLeaderLines = true;

            // Personnalisez les lignes de repère
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
            series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
            series.LeaderLines.Color = Color.LightCyan;

            // Enregistrez le classeur
            workbook.Save("LeaderLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


