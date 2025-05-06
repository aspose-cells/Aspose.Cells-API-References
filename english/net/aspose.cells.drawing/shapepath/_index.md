---
title: Class ShapePath
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapePath class. Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape
type: docs
url: /net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.

```csharp
public class ShapePath
```

## Constructors

| Name | Description |
| --- | --- |
| [ShapePath](shapepath/)() | Initializes a new instance of the `ShapePath` class. |

## Properties

| Name | Description |
| --- | --- |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | Gets [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) list |

## Methods

| Name | Description |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Appends a line segment to the current figure. The starting point is the end point of the current figure. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure. |

### Examples

```csharp
// Called: ShapePath newPath = shapePaths[pathIndex];
public static void Type_ShapePath()
        {



            // Instantiate a new Workbook
            Workbook workbook = new Workbook(&quot;ShapePathCollectionExample_original.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Access the ShapePathCollection of the arc shape
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Add a new path to the ShapePathCollection
                int pathIndex = shapePaths.Add();

                // Access the newly added ShapePath
                ShapePath newPath = shapePaths[pathIndex];

                // Display the count of paths in the ShapePathCollection
                Console.WriteLine(&quot;Number of paths in the ShapePathCollection: &quot; + shapePaths.Count);
            }
            

            // Save the workbook
            workbook.Save(&quot;ShapePathCollectionExample.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


