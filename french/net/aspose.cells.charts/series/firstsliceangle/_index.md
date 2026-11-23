---
title: "Series.FirstSliceAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient ou définit l'angle de la première tranche de piechart ou de doughnutchart en degrés, dans le sens horaire à partir du vertical. S'applique uniquement aux graphiques pie 3D et doughnut avec des valeurs de 0 à 360"
type: docs
url: /fr/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Obtient ou définit l'angle de la première tranche de graphique circulaire ou d'anneau, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux graphiques circulaires, 3D circulaires et en anneau, avec des valeurs de 0 à 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le diagramme circulaire
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique circulaire
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir la première série et définir FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


