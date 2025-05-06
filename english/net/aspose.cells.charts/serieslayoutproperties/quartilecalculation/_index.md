---
title: SeriesLayoutProperties.QuartileCalculation
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Represents the statistical properties for the series
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/quartilecalculation/
---
## SeriesLayoutProperties.QuartileCalculation property

Represents the statistical properties for the series.

```csharp
public QuartileCalculationType QuartileCalculation { get; set; }
```

### Examples

```csharp
// Called: layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;
public static void Property_QuartileCalculation()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Q3&quot;);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Q4&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);
            worksheet.Cells[&quot;B5&quot;].PutValue(40);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add(&quot;B2:B5&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A5&quot;;

            // Access the series layout properties
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Set the quartile calculation type
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Save the workbook
            workbook.Save(&quot;QuartileCalculationTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* enum [QuartileCalculationType](../../quartilecalculationtype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


