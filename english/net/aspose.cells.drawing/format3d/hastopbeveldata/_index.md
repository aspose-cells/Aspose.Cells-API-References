---
title: Format3D.HasTopBevelData
second_title: Aspose.Cells for .NET API Reference
description: Format3D method. Indicates if the shape has top bevel data
type: docs
url: /net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

Indicates if the shape has top bevel data.

```csharp
public bool HasTopBevelData()
```

### Examples

```csharp
// Called: if (format3D.HasTopBevelData())
public static void Method_HasTopBevelData()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(10);
            sheet.Cells[&quot;A2&quot;].PutValue(20);
            sheet.Cells[&quot;A3&quot;].PutValue(30);
            sheet.Cells[&quot;A4&quot;].PutValue(40);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add(&quot;A1:A4&quot;, true);

            // Access the first series
            Series series = chart.NSeries[0];

            // Access the 3D format of the series
            Format3D format3D = series.ShapeProperties.Format3D;

            // Set the 3D format properties
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Check if the shape has top bevel data
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine(&quot;Top Bevel Width: &quot; + topBevel.Width);
                Console.WriteLine(&quot;Top Bevel Height: &quot; + topBevel.Height);
            }

            // Save the workbook
            workbook.Save(&quot;Format3DDemo.xlsx&quot;);
            workbook.Save(&quot;Format3DDemo.pdf&quot;);
        }
```

### See Also

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


