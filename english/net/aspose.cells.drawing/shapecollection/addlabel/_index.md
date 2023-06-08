---
title: ShapeCollection.AddLabel
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Label to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Adds a Label to the worksheet.

```csharp
public Label AddLabel(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Label from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Label, in unit of pixel. |
| width | Int32 | Represents the width of Label, in unit of pixel. |

### Return Value

A Label object.

### Examples

```csharp

[C#]
//add a label
Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
```

### See Also

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


