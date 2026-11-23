---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée x du point final de la section du diagramme circulaire après l'appel de la méthode Chart.Calculate. S'applique aux graphiques en anneau"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Obtient la coordonnée x du point final de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Doughnut.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Ajouter un graphique en anneau
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour obtenir les propriétés des points du graphique
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de InnerArcEndPointXPx
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Remarque : InnerArcEndPointXPx est en lecture seule, nous ne pouvons pas le définir directement
            // Pour modifier la position du point final, nous devons modifier la taille du trou du diagramme en anneau
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Recalculer le graphique pour mettre à jour les propriétés
            chart.Calculate();

            // Afficher la nouvelle valeur de InnerArcEndPointXPx après modification de la taille du trou
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


