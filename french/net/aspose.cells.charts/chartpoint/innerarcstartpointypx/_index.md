---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée y du point de départ de la section du camembert après les appels à la méthode Chart.Calculate. S'applique au graphique en beignet."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Obtient la coordonnée y du point de départ de la section du diagramme circulaire après les appels à la méthode Chart.Calculate(). S'applique au diagramme en anneau.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés sont renseignées
            chart.Calculate();

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur de InnerArcStartPointYPx
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Remarque : InnerArcStartPointYPx est en lecture seule, nous ne pouvons donc pas le définir directement.
            // Pour modifier la position, nous devons ajuster la taille du trou du beignet
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Recalculer le graphique pour mettre à jour les propriétés
            chart.Calculate();

            // Afficher la nouvelle valeur de InnerArcStartPointYPx après modification de la taille du trou
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


