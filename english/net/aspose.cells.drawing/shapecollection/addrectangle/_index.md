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
public RectangleShape AddRectangle(int upperLeftRow, int top, int upperLeftColumn, int left, 
    int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of RectangleShape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of RectangleShape, in unit of pixel. |
| width | Int32 | Represents the width of RectangleShape, in unit of pixel. |

### Return Value

A RectangleShape object.

### Examples

```csharp

[C#]
// add a rectangle
RectangleShape rectangleShape = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
```

### See Also

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


