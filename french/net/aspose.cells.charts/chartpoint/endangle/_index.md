---
title: "ChartPoint.EndAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient l'angle final de la section du diagramme circulaire mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après l'appel de la méthode Chart.Calculate. S'applique au graphique circulaire"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Obtient l'angle final de la section du secteur, mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après l'appel de la méthode Chart.Calculate(). S'applique au graphique Pie.

```csharp
public float EndAngle { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le diagramme circulaire
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés sont renseignées
            chart.Calculate();

            // Obtenir le premier point du graphique (partie Pomme)
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de EndAngle
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Remarque : EndAngle est en lecture seule, nous ne pouvons donc pas le définir directement
            // À la place, nous démontrerons comment il se rapporte à la part du diagramme circulaire

            // Exploser le point pour voir comment cela affecte les angles
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Afficher le nouveau EndAngle après explosion
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Enregistrez le classeur
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


