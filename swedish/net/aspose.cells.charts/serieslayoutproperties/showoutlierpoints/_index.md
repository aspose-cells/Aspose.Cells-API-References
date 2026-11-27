---
title: "SeriesLayoutProperties.ShowOutlierPoints"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Anger om avvikande datapunkter visas"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/showoutlierpoints/
---
## SeriesLayoutProperties.ShowOutlierPoints property

Anger om utliggare datapunkter visas.

```csharp
public bool ShowOutlierPoints { get; set; }
```

### Exempel

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

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(200); // Outlier value
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue("Q2");
            worksheet.Cells["B3"].PutValue("Q3");
            worksheet.Cells["B4"].PutValue("Q4");

            // Skapa ett kolumndiagram (som stödjer avvikande punkter)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.CategoryData = "B1:B4";
            
            // Konfigurera egenskaper för serie layout
            Series series = chart.NSeries[0];
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            
            // Demonstrera ShowOutlierPoints-egenskapen
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.ShowMeanMarker = true;

            workbook.Save("ChartWithOutliers.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


