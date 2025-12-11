---
title: ShapeCollection.AddRectangle
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a RectangleShape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Adds a RectangleShape to the worksheet.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of RectangleShape from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of RectangleShape, in unit of pixel. |
| width | Int32 | Represents the width of RectangleShape, in unit of pixel. |

### Return Value

A RectangleShape object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle using the specified parameters
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Save the workbook
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### See Also

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


