---
title: SeriesCollection.IsColorVaried
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Represents if the color of points is varied
type: docs
url: /net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

Represents if the color of points is varied.

```csharp
public bool IsColorVaried { get; set; }
```

### Remarks

Only works for pie chart or when there is only one series.

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Sample data
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["A5"].PutValue("USA");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);
            cells["B5"].PutValue(85000);

            // Create chart
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Add series
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Set IsColorVaried property
            chart.NSeries.IsColorVaried = true;
            
            // Save the workbook
            workbook.Save("SeriesCollectionPropertyIsColorVariedDemo.xlsx");
        }
    }
}
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


