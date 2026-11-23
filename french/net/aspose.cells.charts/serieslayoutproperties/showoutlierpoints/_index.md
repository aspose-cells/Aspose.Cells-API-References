---
title: "SeriesLayoutProperties.ShowOutlierPoints"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesLayoutProperties. Indique si les points de données aberrants sont affichés"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/showoutlierpoints/
---
## SeriesLayoutProperties.ShowOutlierPoints property

Indique si les points de données aberrants sont affichés.

```csharp
public bool ShowOutlierPoints { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowOutlierPointsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(200); // Outlier value
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue("Q2");
            worksheet.Cells["B3"].PutValue("Q3");
            worksheet.Cells["B4"].PutValue("Q4");

            // Créez un graphique en colonnes (qui prend en charge les points aberrants)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.CategoryData = "B1:B4";
            
            // Configurez les propriétés de disposition de la série
            Series series = chart.NSeries[0];
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            
            // Démontrez la propriété ShowOutlierPoints
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.ShowMeanMarker = true;

            workbook.Save("ChartWithOutliers.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


