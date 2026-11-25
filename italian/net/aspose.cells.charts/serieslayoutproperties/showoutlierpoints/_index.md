---
title: "SeriesLayoutProperties.ShowOutlierPoints"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Indica se i punti dati outlier sono visualizzati"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/showoutlierpoints/
---
## SeriesLayoutProperties.ShowOutlierPoints property

Indica se i punti dati anomali sono mostrati.

```csharp
public bool ShowOutlierPoints { get; set; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(200); // Outlier value
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue("Q2");
            worksheet.Cells["B3"].PutValue("Q3");
            worksheet.Cells["B4"].PutValue("Q4");

            // Crea un grafico a colonne (che supporta i punti outlier)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.CategoryData = "B1:B4";
            
            // Configura le proprietà di layout della serie
            Series series = chart.NSeries[0];
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            
            // Dimostra la proprietà ShowOutlierPoints
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.ShowMeanMarker = true;

            workbook.Save("ChartWithOutliers.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


