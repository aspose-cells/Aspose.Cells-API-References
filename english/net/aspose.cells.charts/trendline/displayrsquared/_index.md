---
title: Trendline.DisplayRSquared
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Represents if the Rsquared value of the trendline is displayed on the chart in the same data label as the equation. Setting this property to True automatically turns on data labels
type: docs
url: /net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

```csharp
public bool DisplayRSquared { get; set; }
```

### Examples

```csharp
// Called: trendline.DisplayRSquared = true;
public static void Property_DisplayRSquared()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Adding a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // Adding a trendline to the first series
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Setting trendline properties
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Saving the Excel file
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
```

### See Also

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


