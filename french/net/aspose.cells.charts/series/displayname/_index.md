---
title: "Series.DisplayName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient le nom de la série qui s'affiche sur le graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Obtient le nom de la série affiché sur le graphique.

```csharp
public string DisplayName { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesPropertyDisplayNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Accéder à la première série et afficher son DisplayName
                Series series = chart.NSeries[0];
                Console.WriteLine("Series DisplayName: " + series.DisplayName);

                // Afficher également la propriété Name pour comparaison
                Console.WriteLine("Series Name: " + series.Name);

                // Enregistrez le classeur
                workbook.Save("DisplayNameDemo.xlsx");
                Console.WriteLine("DisplayName has been demonstrated successfully.");
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

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


