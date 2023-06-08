---
title: ShapeCollection.AddArc
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a ArcShape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Adds a ArcShape to the worksheet.

```csharp
public ArcShape AddArc(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ArcShape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ArcShape, in unit of pixel. |
| width | Int32 | Represents the width of ArcShape, in unit of pixel. |

### Return Value

A ArcShape object.

### Examples

```csharp

[C#]
//add a arc
ArcShape arcShape = shapes.AddArc(1, 0, 1, 0, 100, 50);
```

### See Also

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


