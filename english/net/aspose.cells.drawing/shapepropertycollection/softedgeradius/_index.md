---
title: ShapePropertyCollection.SoftEdgeRadius
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection property. Gets and sets the radius of blur to apply to the edges in unit of points
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/softedgeradius/
---
## ShapePropertyCollection.SoftEdgeRadius property

Gets and sets the radius of blur to apply to the edges, in unit of points.

```csharp
public double SoftEdgeRadius { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePropertyCollectionPropertySoftEdgeRadiusDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionPropertySoftEdgeRadiusDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Display the current SoftEdges value
            Console.WriteLine("Current SoftEdges value: " + shape.SoftEdges);

            // Set a new SoftEdges value (in points)
            shape.SoftEdges = 5.0;
            Console.WriteLine("SoftEdges set to: " + shape.SoftEdges);

            // Add another shape with different SoftEdges for comparison
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 2, 1, 0, 100, 150);
            shape2.SoftEdges = 10.0;

            // Save the workbook to see the effects
            workbook.Save("SoftEdgeRadiusDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


