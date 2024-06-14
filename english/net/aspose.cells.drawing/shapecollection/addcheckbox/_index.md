---
title: ShapeCollection.AddCheckBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a checkbox to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Adds a checkbox to the worksheet.

```csharp
public CheckBox AddCheckBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of checkbox from its top row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | Int32 | Height of textbox, in unit of pixel. |
| width | Int32 | Width of textbox, in unit of pixel. |

### Return Value

The new CheckBox object index.

### Examples

```csharp

[C#]

//add a CheckBox
CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);
```

### See Also

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


