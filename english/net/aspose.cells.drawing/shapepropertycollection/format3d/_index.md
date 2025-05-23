---
title: ShapePropertyCollection.Format3D
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection property. Represents a Format3D object that specifies 3D shape properties for the chart element or shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/format3d/
---
## ShapePropertyCollection.Format3D property

Represents a `Format3D` object that specifies 3D shape properties for the chart element or shape.

```csharp
public Format3D Format3D { get; }
```

### Examples

```csharp
// Called: Format3D format3D = shapeProperties.Format3D;
public static void ShapePropertyCollection_Property_Format3D()
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
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Output the results
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
```

### See Also

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


