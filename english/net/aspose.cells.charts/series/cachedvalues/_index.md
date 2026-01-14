---
title: Series.CachedValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the cached values for the series
type: docs
url: /net/aspose.cells.charts/series/cachedvalues/
---
## Series.CachedValues property

Gets the cached values for the series

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedValues { get; }
```

### Remarks

NOTE: This property is currently for internal use only. It will be changed or removed in next version.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedValuesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Set chart data range
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Access the first series
                Series series = chart.NSeries[0];

                // Display the cached values
                ArrayList cachedValues = series.CachedValues;
                Console.WriteLine("CachedValues count: " + cachedValues.Count);

                // Display each cached value
                for (int i = 0; i < cachedValues.Count; i++)
                {
                    Console.WriteLine("Cached Value " + (i + 1) + ": " + cachedValues[i]);
                }

                // Save the workbook
                workbook.Save("CachedValuesDemo.xlsx");
                Console.WriteLine("CachedValues demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


