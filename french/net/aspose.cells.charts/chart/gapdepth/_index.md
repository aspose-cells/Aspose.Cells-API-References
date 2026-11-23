---
title: "Chart.GapDepth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Obtient ou définit la distance entre les séries de données dans un graphique 3D en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500"
type: docs
url: /fr/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Obtient ou définit la distance entre les séries de données dans un graphique 3D, en pourcentage de la largeur du marqueur. La valeur de cette propriété doit être comprise entre 0 et 500.

```csharp
public int GapDepth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définissez la propriété GapDepth (contrôle la distance entre les séries de données dans les graphiques 3D)
            chart.GapDepth = 150; // Value between 0-500

            // Enregistrez le classeur
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


