---
title: TextBoxCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: TextBoxCollection method. Adds a textbox to the collection
type: docs
url: /net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Adds a textbox to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of textbox, in unit of pixel. |
| width | Int32 | Width of textbox, in unit of pixel. |

### Return Value

[`TextBox`](../../textbox/) object index.

### Examples

```csharp

[C#]
//add a TextBox
int index2 = textBoxCollection.Add(1, 1, 50, 100);
```

### See Also

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


