---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée x du point de départ de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate. S'applique aux graphiques circulaires et en anneau."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Obtient la coordonnée x du point de départ de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

```csharp
public float ArcStartPointXPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés sont renseignées
            chart.Calculate();

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur de ArcStartPointXPx
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Remarque : ArcStartPointXPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // À la place, nous pouvons démontrer comment il change lorsque nous modifions d'autres propriétés

            // Modifiez la valeur d'explosion qui affecte la position de la part du diagramme circulaire
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Afficher la nouvelle valeur de ArcStartPointXPx après modification de l'explosion
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


