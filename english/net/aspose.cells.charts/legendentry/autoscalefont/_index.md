---
title: LegendEntry.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/legendentry/autoscalefont/
---
## LegendEntry.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: firstEntry.AutoScaleFont = true;
public static void Property_AutoScaleFont()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data for the chart
            sheet.Cells[0, 1].PutValue(&quot;Income&quot;);
            sheet.Cells[1, 0].PutValue(&quot;Company A&quot;);
            sheet.Cells[2, 0].PutValue(&quot;Company B&quot;);
            sheet.Cells[3, 0].PutValue(&quot;Company C&quot;);
            sheet.Cells[1, 1].PutValue(10000);
            sheet.Cells[2, 1].PutValue(20000);
            sheet.Cells[3, 1].PutValue(30000);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Access the legend of the chart
            Legend legend = chart.Legend;

            // Access the collection of legend entries
            LegendEntryCollection legendEntries = legend.LegendEntries;

            // Modify properties of the first legend entry
            if (legendEntries.Count &gt; 0)
            {
                LegendEntry firstEntry = legendEntries[0];
                firstEntry.IsDeleted = false;
                firstEntry.AutoScaleFont = true;
                firstEntry.Background = BackgroundMode.Transparent;
            }

            // Save the workbook
            workbook.Save(&quot;LegendEntryCollectionExample.xlsx&quot;);
            workbook.Save(&quot;LegendEntryCollectionExample.pdf&quot;);
        }
```

### See Also

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


