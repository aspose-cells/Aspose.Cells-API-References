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
public static void TickLabels_Property_AlignmentType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access the tick labels of the category axis
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Set the alignment type for the tick labels
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Save the workbook
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [TickLabelAlignmentType](../../ticklabelalignmenttype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


