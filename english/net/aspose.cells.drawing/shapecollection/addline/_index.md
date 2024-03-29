---
title: ShapeCollection.AddLine
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a LineShape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Adds a LineShape to the worksheet.

```csharp
public LineShape AddLine(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of LineShape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of LineShape, in unit of pixel. |
| width | Int32 | Represents the width of LineShape, in unit of pixel. |

### Return Value

A LineShape object.

### Examples

```csharp

[C#]
// add a line object
LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
```

### See Also

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


