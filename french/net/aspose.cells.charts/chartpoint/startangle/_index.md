---
title: "ChartPoint.StartAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient l'angle de départ de la section du diagramme circulaire mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après avoir appelé la méthode Chart.Calculate. S'applique aux diagrammes circulaires."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Obtient l'angle de départ de la section du diagramme circulaire, mesuré en degrés dans le sens des aiguilles d'une montre à partir de l'axe x après l'appel de la méthode Chart.Calculate(). S'applique au diagramme circulaire.

```csharp
public float StartAngle { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
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
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

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

            // Afficher la valeur StartAngle
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Remarque : StartAngle est en lecture seule, nous ne pouvons donc pas le définir directement.
            // Pour modifier l'angle de départ, nous devons faire pivoter l'ensemble du diagramme circulaire.
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Recalculer pour mettre à jour les angles.
            chart.Calculate();

            // Afficher la nouvelle valeur StartAngle après rotation.
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


