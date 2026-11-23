---
title: "ChartPoint.Explosion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. La distance d'une tranche de tarte ouverte du centre du diagramme circulaire est exprimée en pourcentage du diamètre du diagramme"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

La distance d'une tranche de secteur ouverte du centre du graphique en secteurs est exprimée en pourcentage du diamètre du secteur.

```csharp
public int Explosion { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyExplosionDemo
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

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder au premier point du diagramme et définir l'explosion
            ChartPoint point = chart.NSeries[0].Points[0];
            point.Explosion = 15; // Set explosion distance (15 points)

            // Enregistrez le classeur
            workbook.Save("ChartPointExplosionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


