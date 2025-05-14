---
title: FillFormat.PresetColor
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient preset color for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Returns the gradient preset color for the specified fill.

```csharp
public GradientPresetType PresetColor { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);
public static void FillFormat_Property_PresetColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
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

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Access the chart's category axis
            Axis categoryAxis = chart.CategoryAxis;

            // Access the fill format of the category axis area
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Set a gradient preset color for the fill format
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Output the gradient preset color type
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Save the workbook
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
```

### See Also

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


