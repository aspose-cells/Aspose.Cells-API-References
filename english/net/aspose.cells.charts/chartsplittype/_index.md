---
title: Enum ChartSplitType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.ChartSplitType enum. Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split
type: docs
url: /net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.

```csharp
public enum ChartSplitType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Position | `0` | Represents the data points shall be split between the pie and the second chart by putting the last Split Position of the data points in the second chart |
| Value | `1` | Represents the data points shall be split between the pie and the second chart by putting the data points with value less than Split Position in the second chart. |
| PercentValue | `2` | Represents the data points shall be split between the pie and the second chart by putting the points with percentage less than Split Position percent in the second chart. |
| Custom | `3` | Represents the data points shall be split between the pie and the second chart according to the Custom Split values. |
| Auto | `4` | Represents the data points shall be split using the default mechanism for this chart type. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data for the chart
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Add a pie chart
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Set chart data range
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Demonstrate different ChartSplitType values
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Change to another split type
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Save the workbook
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


