---
title: ShapePath.PathSegementList
second_title: Aspose.Cells for .NET API Reference
description: ShapePath property. Gets ShapeSegmentPathCollection list
type: docs
url: /net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Gets [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/) list

```csharp
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePathPropertyPathSegementListDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to access its path (fixed by adding all required parameters)
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 200, 0, 0);
            
            // Get the shape's geometry path (fixed by using Paths instead of ShapePaths)
            ShapePath shapePath = ((CustomGeometry)shape.Geometry).Paths[0];
            
            // Clear existing segments and create a custom path
            shapePath.MoveTo(10, 10);
            shapePath.LineTo(100, 10);
            shapePath.LineTo(100, 100);
            shapePath.LineTo(10, 100);
            shapePath.Close();

            // Access the PathSegementList property
            ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;
            
            // Display the count of path segments
            Console.WriteLine("Number of path segments: " + segmentList.Count);
            
            // Iterate through each segment and display its type
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

            // Save the workbook
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


