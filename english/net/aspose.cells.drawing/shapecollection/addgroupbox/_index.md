---
title: ShapeCollection.AddGroupBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a GroupBox to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Adds a GroupBox to the worksheet.

```csharp
public GroupBox AddGroupBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of GroupBox from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of GroupBox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of GroupBox, in unit of pixel. |
| width | Int32 | Represents the width of GroupBox, in unit of pixel. |

### Return Value

A GroupBox object.

### Examples

```csharp

[C#]
//add a group box
GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);
```

### See Also

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


