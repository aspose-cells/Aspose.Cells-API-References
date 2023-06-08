---
title: ShapeCollection.AddScrollBar
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a ScrollBar to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

Adds a ScrollBar to the worksheet.

```csharp
public ScrollBar AddScrollBar(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ScrollBar from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ScrollBar, in unit of pixel. |
| width | Int32 | Represents the width of ScrollBar, in unit of pixel. |

### Return Value

A ScrollBar object.

### Examples

```csharp

[C#]
//add a scroll bar
ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 1, 0, 100, 50);
```

### See Also

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


