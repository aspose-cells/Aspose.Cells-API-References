---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient le rayon interne de la tranche de beignet en unités de pixels après l'appel de la méthode Chart.Calculate. S'applique au graphique en beignet"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Obtient le rayon interne de la tranche d'anneau en pixels après l'appel de la méthode Chart.Calculate(). S'applique au graphique Doughnut.

```csharp
public int DoughnutInnerRadius { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
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
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Ajouter un graphique en anneau
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculez le graphique pour obtenir les points du graphique
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Affichez la valeur actuelle de DoughnutInnerRadius
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Remarque : DoughnutInnerRadius est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier le rayon interne, nous devons ajuster la propriété HoleSize du graphique
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Recalculez le graphique pour mettre à jour le DoughnutInnerRadius
            chart.Calculate();

            // Affichez la valeur mise à jour de DoughnutInnerRadius
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Enregistrez le classeur
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


