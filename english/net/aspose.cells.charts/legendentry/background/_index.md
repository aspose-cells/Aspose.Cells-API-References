---
title: LegendEntry.Background
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Gets and sets the display mode of the background

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use LegendEntry.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: legendEntry.Background = BackgroundMode.Transparent;
public static void Property_Background()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(200);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            worksheet.Cells[&quot;B4&quot;].PutValue(40);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            worksheet.Cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B4&quot;
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Access the legend entry of the first series
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Set properties of the legend entry
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Access and modify the font of the legend entry
            Font font = legendEntry.Font;
            font.Name = &quot;Arial&quot;;
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Save the workbook
            workbook.Save(&quot;LegendEntryExample.xlsx&quot;);
            workbook.Save(&quot;LegendEntryExample.pdf&quot;);
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


