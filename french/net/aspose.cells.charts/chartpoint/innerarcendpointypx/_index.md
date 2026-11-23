---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée y du point final de la section du camembert après les appels à la méthode Chart.Calculate. S'applique au graphique en beignet."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Obtient la coordonnée y du point final de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Ajouter un graphique en anneau
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour obtenir les propriétés des points du graphique
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de InnerArcEndPointYPx
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Remarque : InnerArcEndPointYPx est en lecture seule, nous ne pouvons donc pas le définir directement.
            // Pour modifier la position, nous devons modifier la taille du trou du beignet
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Recalculer le graphique pour mettre à jour les propriétés
            chart.Calculate();

            // Afficher la nouvelle valeur de InnerArcEndPointYPx après modification de la taille du trou
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


