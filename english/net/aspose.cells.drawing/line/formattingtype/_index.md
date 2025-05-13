---
title: Line.FormattingType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Gets or sets format type
type: docs
url: /net/aspose.cells.drawing/line/formattingtype/
---
## Line.FormattingType property

Gets or sets format type.

```csharp
public ChartLineFormattingType FormattingType { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
public static void Line_Property_FormattingType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Add series to the chart
            chart.NSeries.Add("A1:B3", true);
            
            // Set the category data
            chart.NSeries.CategoryData = "A1:A3";
            
            // Set different line formatting types for the series
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Add another series with different formatting
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Save the workbook
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
```

### See Also

* enum [ChartLineFormattingType](../../../aspose.cells.charts/chartlineformattingtype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


