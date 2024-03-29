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
public Shape AddCopy(Shape sourceShape, int upperLeftRow, int top, int upperLeftColumn, int left)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | Shape | Source shape. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of checkbox from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of textbox from its left column, in unit of pixel. |

### Return Value

The new shape object index.

### Examples

```csharp

[C#]
//add a shape
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//copy
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


