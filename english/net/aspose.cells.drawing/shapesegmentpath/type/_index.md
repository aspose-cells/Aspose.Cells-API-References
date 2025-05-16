---
title: ShapeSegmentPath.Type
second_title: Aspose.Cells for .NET API Reference
description: ShapeSegmentPath property. Gets the path segment type
type: docs
url: /net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Gets the path segment type

```csharp
public ShapePathType Type { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapeSegmentPathPropertyTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a freeform shape with a simple path
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Get the geometry path of the shape
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Add different segment types to demonstrate the Type property
            // Note: Since ShapeSegmentPath has no parameterless constructor and its properties are read-only,
            // we'll need to use the actual segments from the shape path
            Console.WriteLine("\nAll segment types in the path:");
            foreach (ShapeSegmentPath segment in shapePath.PathSegementList)
            {
                Console.WriteLine(segment.Type);
            }

            // Save the workbook
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


