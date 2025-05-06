---
title: Bevel.Type
second_title: Aspose.Cells for .NET API Reference
description: Bevel property. Gets and sets the preset bevel type
type: docs
url: /net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Gets and sets the preset bevel type.

```csharp
public BevelPresetType Type { get; set; }
```

### Examples

```csharp
// Called: topBevel.Type = BevelPresetType.Circle;
public static void Property_Type()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            workbook.CalculateFormula();

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add data series to the chart
            chart.NSeries.Add(&quot;A1:B4&quot;, true);

            // Access the chart&apos;s plot area
            ChartFrame plotArea = chart.PlotArea;

            // Access the shape properties of the plot area
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Access the 3D format properties
            Format3D format3D = shapeProperties.Format3D;

            // Access the top bevel properties
            Bevel topBevel = format3D.TopBevel;

            // Set the width, height, and type of the bevel
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Set other 3D format properties
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Save the workbook
            workbook.Save(&quot;BevelDemo.xlsx&quot;);
            workbook.Save(&quot;BevelDemo.pdf&quot;);
        }
```

### See Also

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


