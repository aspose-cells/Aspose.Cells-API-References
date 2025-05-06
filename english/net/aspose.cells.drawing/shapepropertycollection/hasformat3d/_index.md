---
title: ShapePropertyCollection.HasFormat3D
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Indicates if the shape has 3d format data
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/hasformat3d/
---
## ShapePropertyCollection.HasFormat3D method

Indicates if the shape has 3d format data.

```csharp
public bool HasFormat3D()
```

### Examples

```csharp
// Called: if (shapeProperties.HasFormat3D())
public static void Method_HasFormat3D()
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

            // Access the first series in the chart
            Series series = chart.NSeries[0];

            // Access the shape properties of the series
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Check if the series has 3D format data
            if (shapeProperties.HasFormat3D())
            {
                // Access the 3D format properties
                Format3D format3D = shapeProperties.Format3D;

                // Set the surface lighting type to Balanced
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Set the lighting angle
                format3D.LightingAngle = 45.0;
            }

            // Save the workbook
            workbook.Save(&quot;LightRigTypeExample.xlsx&quot;);
            workbook.Save(&quot;LightRigTypeExample.pdf&quot;);
            // Output the results
            Console.WriteLine(&quot;LightRigType example applied and workbook saved as &apos;LightRigTypeExample.xlsx&apos;.&quot;);
        }
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


