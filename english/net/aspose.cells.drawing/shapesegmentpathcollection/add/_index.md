---
title: ShapeSegmentPathCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ShapeSegmentPathCollection method. Add a segment path in creation path
type: docs
url: /net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Add a segment path in creation path.

```csharp
public int Add(ShapePathType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapePathType | The path type. |

### Return Value

Returns the position of [`ShapeSegmentPath`](../../shapesegmentpath/) object in the list.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a Shape to access its segment paths
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 0, 0, 0, 0, 100, 100);
            
            try
            {
                // Get the ShapeSegmentPathCollection instance
                ShapeSegmentPathCollection segmentPaths = shape.Paths[0].PathSegementList;
                
                // Call Add method with ShapePathType.LineTo
                int index = segmentPaths.Add(ShapePathType.LineTo);
                
                Console.WriteLine($"Segment added at index: {index}");
                
                // Additional segment for demonstration
                segmentPaths.Add(ShapePathType.MoveTo);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Save the workbook to observe the shape modifications
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


