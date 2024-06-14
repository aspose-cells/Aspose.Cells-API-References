---
title: ShapeCollection.AddTextBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a text box to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Adds a text box to the worksheet.

```csharp
public TextBox AddTextBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of textbox, in unit of pixel. |
| width | Int32 | Represents the width of textbox, in unit of pixel. |

### Return Value

A [`TextBox`](../../textbox/) object.

### Examples

```csharp

[C#]

//add a TextBox
TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


