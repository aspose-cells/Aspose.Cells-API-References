---
title: ErrorBar.Amount
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents amount of error bar
type: docs
url: /net/aspose.cells.charts/errorbar/amount/
---
## ErrorBar.Amount property

Represents amount of error bar.

```csharp
public double Amount { get; set; }
```

### Remarks

The amount must be greater than or equal to zero.

### Examples

```csharp
// Called: series.YErrorBar.Amount = 5;
public static void Property_Amount()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Add some sample data
            cells[&quot;A1&quot;].PutValue(2);
            cells[&quot;A2&quot;].PutValue(5);
            cells[&quot;A3&quot;].PutValue(3);
            cells[&quot;A4&quot;].PutValue(6);
            cells[&quot;B1&quot;].PutValue(4);
            cells[&quot;B2&quot;].PutValue(3);
            cells[&quot;B3&quot;].PutValue(6);
            cells[&quot;B4&quot;].PutValue(7);

            cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Add a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Set error bar properties for each series in the chart
            for (int i = 0; i &lt; chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Save the workbook
            workbook.Save(&quot;ErrorBarTypeExample.xlsx&quot;);
            workbook.Save(&quot;ErrorBarTypeExample.pdf&quot;);
        }
```

### See Also

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


