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
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add("A1:A4", true);

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
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Save the workbook
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
```

### See Also

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


