---
title: "ChartPoint.InnerRadiusPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient le rayon interne de la tranche d'anneau en unités de pixels après l'appel de la méthode Chart.Calculate. S'applique au graphique en anneau"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Obtient le rayon interne de la tranche d'anneau en unités de pixels après l'appel de la méthode Chart.Calculate(). S'applique au graphique en anneau.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartPoint.DoughnutInnerRadius. Cette propriété sera supprimée 12 mois après, depuis juin 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour obtenir les propriétés des points du graphique
            chart.Calculate();

            // Obtenir le premier point du graphique de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle du rayon interne (propriété en lecture seule)
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Remarque : InnerRadiusPx est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour modifier le rayon interne, nous devons ajuster la taille du trou de l'anneau
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Recalculer le graphique pour mettre à jour les propriétés
            chart.Calculate();

            // Afficher la nouvelle valeur du rayon interne après avoir ajusté la taille du trou de l'anneau
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Enregistrer le résultat
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


