---
title: "Series.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Vrai si la série a une ombre"
type: docs
url: /fr/net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

Vrai si la série possède une ombre.

```csharp
public bool Shadow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez à la première série et activez l'ombre
            Series series = chart.NSeries[0];
            series.Shadow = true;

            // Enregistrez et rechargez pour vérifier
            workbook.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Series loadedSeries = loadedWorkbook.Worksheets[0].Charts[0].NSeries[0];
            Console.WriteLine("Shadow enabled: " + loadedSeries.Shadow);
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


