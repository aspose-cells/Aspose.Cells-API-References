---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée y du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate. S'applique aux graphiques circulaires et en anneau"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Obtient la coordonnée y du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

```csharp
public float ArcStartPointYPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour obtenir les positions des formes
            chart.Calculate();

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de ArcStartPointYPx
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Remarque : ArcStartPointYPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // À la place, nous allons démontrer comment la modification d'autres propriétés affecte ArcStartPointYPx

            // Modifiez la valeur d'explosion pour modifier la position de la part du diagramme circulaire
            point.Explosion = 20;

            // Recalculez le graphique pour mettre à jour les positions
            chart.Calculate();

            // Affichez la nouvelle valeur de ArcStartPointYPx après avoir modifié l'explosion
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


