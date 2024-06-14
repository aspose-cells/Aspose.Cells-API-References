---
title: ShapeCollection.AddCopy
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds and copy a shape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addcopy/
---
## ShapeCollection.AddCopy method

Adds and copy a shape to the worksheet.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | Shape | Source shape. |
| topRow | Int32 | The top row index. |
| top | Int32 | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | Int32 | The left column index. |
| left | Int32 | Represents the horizontal offset from its left column, in unit of pixel. |

### Return Value

The new [`Shape`](../../shape/) object.

### Examples

```csharp

[C#]
//add a shape
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Adds and copies a shape.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


