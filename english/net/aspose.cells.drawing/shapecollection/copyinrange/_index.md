---
title: ShapeCollection.CopyInRange
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Copy shapes in the range to destination range
type: docs
url: /net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Copy shapes in the range to destination range.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Source shapes. |
| ca | CellArea | The source range. |
| destRow | Int32 | The dest row index of the dest range. |
| destColumn | Int32 | The dest column of the dest range. |
| isContained | Boolean | Whether only copy the shapes which are contained in the range. If true,only copies the shapes in the range. Otherwise,it works as MS Office. |

### Examples

```csharp

[C#]
//add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
CellArea area2 = new CellArea();
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;

//copy
shapes.CopyInRange(shapes, area2, 12, 1, false);

```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


