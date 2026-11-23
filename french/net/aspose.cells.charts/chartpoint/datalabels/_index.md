---
title: "ChartPoint.DataLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Retourne un objet DataLabels qui représente l'étiquette de données associée à ce point de graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Retourne un objet `DataLabels` qui représente l'étiquette de données associée à ce point de graphique.

```csharp
public DataLabels DataLabels { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDataLabelsDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accéder au premier point du graphique
                ChartPoint point = chart.NSeries[0].Points[0];

                // Obtenir la propriété DataLabels (lecture seule)
                DataLabels dataLabels = point.DataLabels;

                // Afficher les propriétés de DataLabels
                Console.WriteLine("DataLabels ShowValue: " + dataLabels.ShowValue);
                Console.WriteLine("DataLabels ShowCategoryName: " + dataLabels.ShowCategoryName);
                Console.WriteLine("DataLabels ShowSeriesName: " + dataLabels.ShowSeriesName);
                Console.WriteLine("DataLabels Position: " + dataLabels.Position);

                // Modifier certaines propriétés de DataLabels (puisque DataLabels n'est pas en lecture seule)
                dataLabels.ShowValue = true;
                dataLabels.ShowCategoryName = true;
                dataLabels.Position = LabelPositionType.OutsideEnd;

                // Enregistrer le résultat
                workbook.Save("ChartPointDataLabelsDemo.xlsx");
                Console.WriteLine("DataLabels demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


