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
// Called: Console.WriteLine(&amp;quot;Gradient Preset Color: &amp;quot; + fillFormat.PresetColor);
public static void Property_PresetColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
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

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Access the chart&apos;s category axis
            Axis categoryAxis = chart.CategoryAxis;

            // Access the fill format of the category axis area
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Set a gradient preset color for the fill format
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Output the gradient preset color type
            Console.WriteLine(&quot;Gradient Preset Color: &quot; + fillFormat.PresetColor);

            // Save the workbook
            workbook.Save(&quot;GradientPresetTypeExample.xlsx&quot;);
            workbook.Save(&quot;GradientPresetTypeExample.pdf&quot;);
        }
```

### See Also

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


