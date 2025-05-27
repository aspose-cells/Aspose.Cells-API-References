---
title: ShapeSegmentPathCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ShapeSegmentPathCollection property. Gets ShapeSegmentPath object
type: docs
url: /net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Gets [`ShapeSegmentPath`](../../shapesegmentpath/) object.

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

Returns a [`ShapeSegmentPath`](../../shapesegmentpath/) object.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a shape to access its segment paths
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 0, 0, 100, 100, 0, 0);
            
            // Get the ShapeSegmentPathCollection instance
            ShapeSegmentPathCollection segmentPaths = shape.Paths[0].PathSegementList;
            
            // Add some path segments
            segmentPaths.Add(ShapePathType.MoveTo);
            segmentPaths.Add(ShapePathType.LineTo);
            segmentPaths.Add(ShapePathType.CubicBezierCurveTo);
            
            // Demonstrate reading the Item property
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }
            
            // Note: The Item property is read-only, so we can't set it directly
            // Instead, we can modify the segments by accessing their properties
            if (segmentPaths.Count > 0)
            {
                ShapeSegmentPath firstSegment = segmentPaths[0];
                Console.WriteLine($"First segment before modification: {firstSegment.Type}");
                
                // This demonstrates that while we can't replace the entire segment,
                // we can modify its properties if they are writable
                // (Note: ShapeSegmentPath.Type is read-only in this case)
            }
            
            // Save the workbook
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


