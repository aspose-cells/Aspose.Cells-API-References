---
title: "Series.LayoutProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar layoutens egenskaper"
type: docs
url: /sv/net/aspose.cells.charts/series/layoutproperties/
---
## Series.LayoutProperties property

Representerar layoutens egenskaper.

```csharp
public SeriesLayoutProperties LayoutProperties { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLayoutPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldatat för låd- och whisker-diagram
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q1");
            sheet.Cells["A4"].PutValue("Q1");
            sheet.Cells["A5"].PutValue("Q2");
            sheet.Cells["A6"].PutValue("Q2");
            sheet.Cells["A7"].PutValue("Q2");

            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(15);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(20);
            sheet.Cells["B6"].PutValue(35);
            sheet.Cells["B7"].PutValue(40);

            // Lägg till låd- och whisker-diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.BoxWhisker, 5, 0, 25, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("B1:B7", true);
            chart.NSeries.CategoryData = "A2:A7";

            // Konfigurera layoutinställningar för serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.LayoutProperties.ShowMeanLine = false;
            series.LayoutProperties.ShowInnerPoints = true;
            series.LayoutProperties.ShowOutlierPoints = true;
            series.LayoutProperties.ShowMeanMarker = true;

            // Spara arbetsboken
            workbook.Save("SeriesLayoutPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../../serieslayoutproperties/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


