---
title: ShapeCollection.AddAutoShape
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a AutoShape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Adds a AutoShape to the worksheet.

```csharp
public Shape AddAutoShape(AutoShapeType type, int upperLeftRow, int top, int upperLeftColumn, 
    int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Auto shape type. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Shape, in unit of pixel. |
| width | Int32 | Represents the width of Shape, in unit of pixel. |

### Return Value

A Shape object.

### Remarks

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Examples

```csharp

[C#]
//Adds a AutoShape to the worksheet.
Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
```

### See Also

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


