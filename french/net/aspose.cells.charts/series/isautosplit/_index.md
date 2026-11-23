---
title: "Series.IsAutoSplit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Indique si la valeur du seuil est automatique"
type: docs
url: /fr/net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

Indique si la valeur du seuil est automatique.

```csharp
public bool IsAutoSplit { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsAutoSplitDemo
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
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accédez à la première série et démontrez la propriété IsAutoSplit
            Series series = chart.NSeries[0];
            bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
            series.SplitValue = 25; // Split at value 25

            Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");

            // Enregistrez le classeur
            workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


