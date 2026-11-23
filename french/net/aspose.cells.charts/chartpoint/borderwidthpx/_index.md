---
title: "ChartPoint.BorderWidthPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la largeur de la bordure en unités de pixels après l'appel de la méthode Chart.Calculate."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Obtient la largeur de la bordure en pixels après l'appel de la méthode Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
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
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calculer le graphique pour garantir que les propriétés sont renseignées
            chart.Calculate();

            // Obtenir le premier point du graphique dans la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la largeur de bordure actuelle
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Remarque : BorderWidthPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // À la place, nous pouvons modifier la bordure via la propriété Border
            if (point.Border != null)
            {
                // Modifiez la largeur de la bordure en définissant le poids à l'aide de l'énumération WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Recalculer pour mettre à jour la valeur de BorderWidthPx
            chart.Calculate();

            // Afficher la nouvelle largeur de bordure en pixels
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


