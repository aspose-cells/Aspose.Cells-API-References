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
// Called: Format3D format3D = series.ShapeProperties.Format3D;
public static void Property_Format3D()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Access the first series in the chart
            Series series = chart.NSeries[0];

            // Access the 3D format of the series
            Format3D format3D = series.ShapeProperties.Format3D;

            // Set the surface material type
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Set other 3D properties
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Save the workbook
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Output the results
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
```

### See Also

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


