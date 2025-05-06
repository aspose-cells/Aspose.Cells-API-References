---
title: TickLabels.AlignmentType
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Gets and sets the text alignment for the tick labels on the axis
type: docs
url: /net/aspose.cells.charts/ticklabels/alignmenttype/
---
## TickLabels.AlignmentType property

Gets and sets the text alignment for the tick labels on the axis.

```csharp
public TickLabelAlignmentType AlignmentType { get; set; }
```

### Examples

```csharp
// Called: tickLabels.AlignmentType = TickLabelAlignmentType.Center;
public static void Property_AlignmentType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

            // Access the tick labels of the category axis
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Set the alignment type for the tick labels
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Save the workbook
            workbook.Save(&quot;TickLabelAlignmentTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* enum [TickLabelAlignmentType](../../ticklabelalignmenttype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


